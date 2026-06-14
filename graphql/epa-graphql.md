# EPA — U.S. Environmental Protection Agency GraphQL API

## Overview

The U.S. Environmental Protection Agency (EPA) does not currently publish a native public GraphQL endpoint. The EPA exposes its environmental data through REST and SOAP services across programs including Envirofacts, ECHO (Enforcement and Compliance History Online), AQS (Air Quality System), FRS (Facility Registry Service), EJScreen, TRI (Toxics Release Inventory), Superfund/SEMS, SDWIS (Safe Drinking Water Information System), RCRA Info, and GHGRP (Greenhouse Gas Reporting Program).

This document defines a conceptual GraphQL schema that unifies those REST services into a coherent graph. Clients could use this schema as the basis for a GraphQL gateway or federation layer that wraps EPA's existing endpoints.

## Source APIs

| Program | Base URL | Description |
|---------|----------|-------------|
| AQS Data Mart | `https://aqs.epa.gov/data/api` | Ambient air-quality monitoring data |
| Envirofacts | `https://data.epa.gov/efservice` | Cross-program data warehouse (TRI, GHG, RCRA, SDWIS, SEMS, NEI) |
| ECHO | `https://echodata.epa.gov/echo` | Facility compliance and enforcement history |
| FRS | `https://ofmpub.epa.gov/frs_public2` | Facility Registry Service |
| EJScreen | `https://ejscreen.epa.gov/mapper/ejscreenRESTbroker.aspx` | Environmental justice screening indices |
| GHGRP | `https://enviro.epa.gov/query-builder/api` | Greenhouse gas facility-level data |

## Schema File

See [`epa-schema.graphql`](epa-schema.graphql) for the full type definitions.

## Key Domain Areas

### Air Quality (AQS / NAAQS)
- `AirQualityStation` — monitoring station identity, coordinates, operating agency
- `AirMonitor` — individual instrument within a station (method, parameter, span)
- `AirQualityReading` — raw or aggregated sample measurement
- `AQICategory` — Good / Moderate / Unhealthy breakpoints per NAAQS
- `Pollutant` — EPA parameter code, CAS number, standard units
- `PollutantLevel` — measured concentration with uncertainty
- `NAAQS` — primary/secondary standard, averaging period
- `AirEmission` — point-source emission inventory quantity (NEI)
- `CAAPermit` — Clean Air Act Title V / minor-source permit

### Water Quality (ECHO CWA / SDWIS)
- `WaterBody` — named stream, lake, or estuary with classification
- `WaterQualitySample` — field sample with analyte results
- `WaterPermit` — general NPDES or individual permit record
- `NPDESPermit` — detailed permit with limits, outfalls, schedules
- `DischargeMonitoringReport` — DMR submission with parameter exceedances
- `SDWASystem` — public water system identity and classification
- `SDWASample` — drinking-water sample with contaminant results
- `LeadCopper` — 90th-percentile lead/copper monitoring result
- `UICWell` — underground injection control well record

### Hazardous Waste (RCRA)
- `RCRAFacility` — handler/generator/TSD site under RCRA
- `HazardousWasteManifest` — manifest tracking from cradle to grave

### Toxics Release Inventory (TRI)
- `ToxicsReleaseInventory` — facility-level TRI submission year
- `TRIReport` — annual Form R or Form A report
- `TRIChemical` — chemical released with quantity by release path
- `ChemicalFacility` — facility reporting under Section 313

### Superfund / Cleanup (CERCLA / SEMS)
- `SuperfundSite` — NPL or non-NPL CERCLA site
- `CleanupStatus` — current remedial phase and milestone
- `CleanupAction` — individual response action at a site

### Greenhouse Gas Reporting
- `GHGFacility` — large stationary source under 40 CFR Part 98
- `GHGEmission` — reported CO2-equivalent by subpart

### Facility Registry
- `FacilityRegistryRecord` — master facility record across all EPA programs
- `FacilityLocation` — geocoded address and coordinates

### Compliance and Enforcement (ECHO)
- `ComplianceRecord` — quarterly compliance status per program
- `InspectionRecord` — inspection date, type, and findings
- `Violation` — specific regulatory violation instance
- `EnforcementAction` — formal or informal enforcement activity
- `Penalty` — assessed and paid penalty amounts

### Environmental Justice (EJScreen)
- `EJScreen` — block-group-level EJ index composite
- `DemographicData` — census demographic variables for a geography
- `EnvironmentalIndex` — individual environmental burden indicator
- `HealthRisk` — cancer or non-cancer risk estimate

### Climate
- `ClimateIndicator` — EPA-tracked climate change indicator time series

## Example Query

```graphql
query FacilityOverview($registryId: ID!) {
  facilityRegistryRecord(registryId: $registryId) {
    facilityName
    location {
      streetAddress
      city
      state
      latitude
      longitude
    }
    npdesPermits {
      permitNumber
      permitType
      issueDate
      expirationDate
      dischargeMonitoringReports(year: 2023) {
        reportingPeriod
        parameterName
        measuredValue
        limitValue
        exceedance
      }
    }
    triReports(year: 2022) {
      triChemicals {
        chemicalName
        casNumber
        totalAirEmissionsLbs
        totalWaterDischargesLbs
        totalLandfillDisposalLbs
      }
    }
    ejScreen {
      pm25Percentile
      ozonePercentile
      dieselPmPercentile
      cancerRiskPercentile
      lowIncomePercentile
      peopleOfColorPercentile
    }
    complianceRecords(programs: [CAA, CWA, RCRA]) {
      program
      quarterlyStatus
      violations {
        violationType
        violationDate
        resolvedDate
      }
    }
  }
}
```

## References

- EPA Developers Hub: https://www.epa.gov/developers
- ECHO Web Services: https://echo.epa.gov/tools/web-services
- AQS Data Mart API: https://aqs.epa.gov/aqsweb/documents/data_api.html
- Envirofacts API: https://www.epa.gov/enviro/envirofacts-data-service-api
- EJScreen REST API: https://www.epa.gov/ejscreen/ejscreen-api
- GHGRP Data: https://www.epa.gov/ghgreporting/ghg-reporting-program-data-sets
- GitHub: https://github.com/USEPA
