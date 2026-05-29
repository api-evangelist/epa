# EPA — U.S. Environmental Protection Agency (epa)

Web services, data products, and open data spanning the U.S. Environmental Protection Agency. Programmatic access to air quality, water quality, hazardous waste, toxic releases, facility compliance, power-sector emissions, computational toxicology, and watershed assessments through dozens of public APIs.

**URL:** [https://www.epa.gov/developers/data-data-products](https://www.epa.gov/developers/data-data-products)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Type
- **x-type:** government
- **x-tier:** 1 (enriched-with-full-pipeline)
- **x-category:** Government

## Tags
- Government, Environmental, OpenData, AirQuality, WaterQuality, HazardousWaste, Compliance, Emissions

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Artifact Inventory
- **OpenAPI specifications:** 22
- **JSON Schema files:** 621
- **JSON Structure files:** 621
- **JSON-LD context files:** 23
- **Example payloads:** 621
- **Naftiko capabilities:** 151
- **Spectral rulesets:** 1
- **Vocabulary files:** 1
- **Rate-limit artifacts:** 1

## APIs

### AQS — Air Quality System Data Mart API

Programmatic access to ambient air pollution monitoring data — sites, monitors, sample/daily/quarterly/annual aggregates, and quality assurance results for criteria and hazardous air pollutants.

- **Base URL:** `https://aqs.epa.gov/data/api`
- **Documentation:** [https://aqs.epa.gov/aqsweb/documents/data_api.html](https://aqs.epa.gov/aqsweb/documents/data_api.html)
- **Tags:** Government, Environmental, AirQuality, Monitoring
- **OpenAPI:** 1 spec(s) — [aqs-openapi.yml](openapi/aqs-openapi.yml)
- **Naftiko Capabilities:** 10 file(s)
- **JSON Schemas:** 2 file(s)
- **JSON Structures:** 2 file(s)
- **Examples:** 2 payload(s)

### Envirofacts Data Service API

EPA's cross-program REST data warehouse covering RCRA, GHG, TRI, SEMS, NEI, SDWIS and more, plus a GraphQL endpoint and UV index forecast feeds.

- **Base URL:** `https://data.epa.gov`
- **Documentation:** [https://www.epa.gov/enviro/envirofacts-data-service-api](https://www.epa.gov/enviro/envirofacts-data-service-api)
- **Tags:** Government, Environmental, OpenData, UVIndex
- **OpenAPI:** 1 spec(s) — [envirofacts-openapi.yml](openapi/envirofacts-openapi.yml)
- **Naftiko Capabilities:** 3 file(s)
- **JSON Schemas:** 3 file(s)
- **JSON Structures:** 3 file(s)
- **Examples:** 3 payload(s)

### ECHO — All Media Programs Facility Search

Cross-program facility compliance search returning regulated facilities across air, water, waste, and drinking-water programs.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services](https://echo.epa.gov/tools/web-services)
- **Tags:** Government, Compliance, Facilities
- **OpenAPI:** 1 spec(s) — [echo-all-openapi.json](openapi/echo-all-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 15 file(s)
- **JSON Structures:** 15 file(s)
- **Examples:** 15 payload(s)

### ECHO — Clean Air Act Facility Search

CAA stationary-source facility compliance search.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services/facility-search-air](https://echo.epa.gov/tools/web-services/facility-search-air)
- **Tags:** Government, AirQuality, Compliance
- **OpenAPI:** 1 spec(s) — [echo-air-openapi.json](openapi/echo-air-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 16 file(s)
- **JSON Structures:** 16 file(s)
- **Examples:** 16 payload(s)

### ECHO — Clean Water Act Facility Search

NPDES wastewater, stormwater, and biosolids discharger search and compliance data.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services/facility-search-water](https://echo.epa.gov/tools/web-services/facility-search-water)
- **Tags:** Government, WaterQuality, Compliance
- **OpenAPI:** 1 spec(s) — [echo-cwa-openapi.json](openapi/echo-cwa-openapi.json)
- **Naftiko Capabilities:** 3 file(s)
- **JSON Schemas:** 28 file(s)
- **JSON Structures:** 28 file(s)
- **Examples:** 28 payload(s)

### ECHO — Safe Drinking Water Act System Search

SDWA public water system search and compliance reporting.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services/facility-search-drinking-water](https://echo.epa.gov/tools/web-services/facility-search-drinking-water)
- **Tags:** Government, DrinkingWater, Compliance
- **OpenAPI:** 1 spec(s) — [echo-sdw-openapi.json](openapi/echo-sdw-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 5 file(s)
- **JSON Structures:** 5 file(s)
- **Examples:** 5 payload(s)

### ECHO — RCRA Hazardous Waste Facility Search

RCRA hazardous waste generator/handler/TSD facility search and compliance data.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services/facility-search-hazardous-waste](https://echo.epa.gov/tools/web-services/facility-search-hazardous-waste)
- **Tags:** Government, HazardousWaste, Compliance
- **OpenAPI:** 1 spec(s) — [echo-rcra-openapi.json](openapi/echo-rcra-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 17 file(s)
- **JSON Structures:** 17 file(s)
- **Examples:** 17 payload(s)

### ECHO — Enforcement Case Search

Civil and criminal enforcement case search and reporting.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/tools/web-services/enforcement-case-search](https://echo.epa.gov/tools/web-services/enforcement-case-search)
- **Tags:** Government, Enforcement, Compliance
- **OpenAPI:** 1 spec(s) — [echo-case-openapi.json](openapi/echo-case-openapi.json)
- **Naftiko Capabilities:** 3 file(s)
- **JSON Schemas:** 41 file(s)
- **JSON Structures:** 41 file(s)
- **Examples:** 41 payload(s)

### ECHO — Detailed Facility Report

Comprehensive 5-year compliance and enforcement history for a single facility, spanning every program ECHO indexes.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/detailed-facility-report](https://echo.epa.gov/detailed-facility-report)
- **Tags:** Government, Facilities, Compliance
- **OpenAPI:** 1 spec(s) — [echo-dfr-openapi.json](openapi/echo-dfr-openapi.json)
- **Naftiko Capabilities:** 1 file(s)
- **JSON Schemas:** 156 file(s)
- **JSON Structures:** 156 file(s)
- **Examples:** 156 payload(s)

### ECHO — Effluent Charting and Reporting

NPDES permit effluent monitoring time-series charts and download services.

- **Base URL:** `https://echodata.epa.gov`
- **Documentation:** [https://echo.epa.gov/trends/loading-tool/water-pollution-search](https://echo.epa.gov/trends/loading-tool/water-pollution-search)
- **Tags:** Government, WaterQuality, Enforcement
- **OpenAPI:** 1 spec(s) — [echo-effluent-openapi.json](openapi/echo-effluent-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 11 file(s)
- **JSON Structures:** 11 file(s)
- **Examples:** 11 payload(s)

### CAM — Account Management

Clean Air Markets account holdings, allowance transactions, and compliance positions.

- **Base URL:** `https://api.epa.gov/easey/account-mgmt`
- **Documentation:** [https://api.epa.gov/easey/account-mgmt/swagger](https://api.epa.gov/easey/account-mgmt/swagger)
- **Tags:** Government, PowerSector, Emissions
- **OpenAPI:** 1 spec(s) — [cam-account-openapi.json](openapi/cam-account-openapi.json)
- **Naftiko Capabilities:** 6 file(s)
- **JSON Schemas:** 12 file(s)
- **JSON Structures:** 12 file(s)
- **Examples:** 12 payload(s)

### CAM — CAMD Administrative & General Services

Clean Air Markets prepackaged bulk datasets and admin services.

- **Base URL:** `https://api.epa.gov/easey/camd-services`
- **Documentation:** [https://api.epa.gov/easey/camd-services/swagger](https://api.epa.gov/easey/camd-services/swagger)
- **Tags:** Government, PowerSector, BulkData
- **OpenAPI:** 1 spec(s) — [cam-camd-services-openapi.json](openapi/cam-camd-services-openapi.json)
- **Naftiko Capabilities:** 4 file(s)
- **JSON Schemas:** 6 file(s)
- **JSON Structures:** 6 file(s)
- **Examples:** 6 payload(s)

### CAM — Emissions Management

Continuous emissions monitoring data submission and retrieval for fossil power plants.

- **Base URL:** `https://api.epa.gov/easey/emissions-mgmt`
- **Documentation:** [https://api.epa.gov/easey/emissions-mgmt/swagger](https://api.epa.gov/easey/emissions-mgmt/swagger)
- **Tags:** Government, PowerSector, Emissions
- **OpenAPI:** 1 spec(s) — [cam-emissions-openapi.json](openapi/cam-emissions-openapi.json)
- **Naftiko Capabilities:** 12 file(s)
- **JSON Schemas:** 31 file(s)
- **JSON Structures:** 31 file(s)
- **Examples:** 31 payload(s)

### CAM — Facilities Management

Power plant facility, unit, stack, and owner attributes for CAM-regulated sources.

- **Base URL:** `https://api.epa.gov/easey/facilities-mgmt`
- **Documentation:** [https://api.epa.gov/easey/facilities-mgmt/swagger](https://api.epa.gov/easey/facilities-mgmt/swagger)
- **Tags:** Government, PowerSector, Facilities
- **OpenAPI:** 1 spec(s) — [cam-facilities-openapi.json](openapi/cam-facilities-openapi.json)
- **Naftiko Capabilities:** 2 file(s)
- **JSON Schemas:** 3 file(s)
- **JSON Structures:** 3 file(s)
- **Examples:** 3 payload(s)

### CAM — Master Data Management

Lookup codes and reference data spanning the CAM domain.

- **Base URL:** `https://api.epa.gov/easey/master-data-mgmt`
- **Documentation:** [https://api.epa.gov/easey/master-data-mgmt/swagger](https://api.epa.gov/easey/master-data-mgmt/swagger)
- **Tags:** Government, PowerSector, MasterData
- **OpenAPI:** 1 spec(s) — [cam-master-data-openapi.json](openapi/cam-master-data-openapi.json)
- **Naftiko Capabilities:** 9 file(s)
- **JSON Schemas:** 10 file(s)
- **JSON Structures:** 10 file(s)
- **Examples:** 10 payload(s)

### CAM — Monitoring Plan Management

Continuous emissions monitoring plan retrieval and submission.

- **Base URL:** `https://api.epa.gov/easey/monitor-plan-mgmt`
- **Documentation:** [https://api.epa.gov/easey/monitor-plan-mgmt/swagger](https://api.epa.gov/easey/monitor-plan-mgmt/swagger)
- **Tags:** Government, PowerSector, Emissions
- **OpenAPI:** 1 spec(s) — [cam-monitor-plan-openapi.json](openapi/cam-monitor-plan-openapi.json)
- **Naftiko Capabilities:** 28 file(s)
- **JSON Schemas:** 64 file(s)
- **JSON Structures:** 64 file(s)
- **Examples:** 64 payload(s)

### CAM — QA & Certifications Management

Quality assurance test and certification data for CAM-regulated emissions monitoring systems.

- **Base URL:** `https://api.epa.gov/easey/qa-certification-mgmt`
- **Documentation:** [https://api.epa.gov/easey/qa-certification-mgmt/swagger](https://api.epa.gov/easey/qa-certification-mgmt/swagger)
- **Tags:** Government, PowerSector, QualityAssurance
- **OpenAPI:** 1 spec(s) — [cam-qa-cert-openapi.json](openapi/cam-qa-cert-openapi.json)
- **Naftiko Capabilities:** 33 file(s)
- **JSON Schemas:** 57 file(s)
- **JSON Structures:** 57 file(s)
- **Examples:** 57 payload(s)

### CAM — Streaming Services

High-throughput streaming endpoints for accounts, allowances, facilities, and apportioned/raw emissions.

- **Base URL:** `https://api.epa.gov/easey/streaming-services`
- **Documentation:** [https://api.epa.gov/easey/streaming-services/swagger](https://api.epa.gov/easey/streaming-services/swagger)
- **Tags:** Government, PowerSector, Streaming
- **OpenAPI:** 1 spec(s) — [cam-streaming-openapi.json](openapi/cam-streaming-openapi.json)
- **Naftiko Capabilities:** 15 file(s)
- **JSON Schemas:** 35 file(s)
- **JSON Structures:** 35 file(s)
- **Examples:** 35 payload(s)

### CIP — Catchment Index Processing Service

StreamCat / LakeCat catchment indexing and metric services.

- **Base URL:** `https://cipservice.app.cloud.gov`
- **Documentation:** [https://github.com/USEPA/CIP-service](https://github.com/USEPA/CIP-service)
- **Tags:** Government, Watersheds, GIS
- **OpenAPI:** 1 spec(s) — [cip-service-openapi.yml](openapi/cip-service-openapi.yml)
- **Naftiko Capabilities:** 3 file(s)
- **JSON Schemas:** 82 file(s)
- **JSON Structures:** 82 file(s)
- **Examples:** 82 payload(s)

### CSB — Clean School Bus Rebate Forms

Internal-facing API for the Clean School Bus rebate program — eligibility, applications, and award tracking.

- **Base URL:** `https://www.epa.gov/cleanschoolbus`
- **Documentation:** [https://github.com/USEPA/csb-rebate-forms-app](https://github.com/USEPA/csb-rebate-forms-app)
- **Tags:** Government, Transportation, Rebates
- **OpenAPI:** 1 spec(s) — [csb-rebate-openapi.json](openapi/csb-rebate-openapi.json)
- **Naftiko Capabilities:** 1 file(s)
- **JSON Schemas:** 1 file(s)
- **JSON Structures:** 1 file(s)
- **Examples:** 1 payload(s)

### ELG — Effluent Guidelines Search

WaterSense Effluent Limitations Guidelines search across point source categories, pollutants, and treatment technologies.

- **Base URL:** `https://owapps.epa.gov/elg-search-tools-api`
- **Documentation:** [https://www.epa.gov/eg](https://www.epa.gov/eg)
- **Tags:** Government, WaterQuality, WaterSense
- **OpenAPI:** 1 spec(s) — [elg-search-openapi.json](openapi/elg-search-openapi.json)
- **Naftiko Capabilities:** 7 file(s)
- **JSON Schemas:** 25 file(s)
- **JSON Structures:** 25 file(s)
- **Examples:** 25 payload(s)

### How's My Waterway

Public access to local water quality status (rivers, lakes, beaches, drinking water) via the ATTAINS data layer.

- **Base URL:** `https://mywaterway.epa.gov/api`
- **Documentation:** [https://mywaterway.epa.gov](https://mywaterway.epa.gov)
- **Tags:** Government, WaterQuality, PublicAccess
- **OpenAPI:** 1 spec(s) — [mywaterway-openapi.json](openapi/mywaterway-openapi.json)
- **Naftiko Capabilities:** 1 file(s)
- **JSON Schemas:** 1 file(s)
- **JSON Structures:** 1 file(s)
- **Examples:** 1 payload(s)

### EPA Facility Registry Service (FRS) API

Master inventory of EPA-regulated facilities cross-walked across air, water, waste, and drinking-water programs. Production query and submit endpoints require a NAAS account.

- **Base URL:** `https://frsqueryprd-api.epa.gov/facilityiptqueryprd`
- **Documentation:** [https://www.epa.gov/frs/facility-registry-service-frs-api](https://www.epa.gov/frs/facility-registry-service-frs-api)
- **Tags:** Government, Facilities, MasterData

### EPA TRI (Toxics Release Inventory) Web Service

Toxic chemical release and transfer reporting (Form R / Form A) covering ~770 listed chemicals at TRI-covered facilities. Exposed primarily via the Envirofacts data service over the `tri.*` tables.

- **Base URL:** `https://data.epa.gov/efservice/tri`
- **Documentation:** [https://www.epa.gov/enviro/tri-customized-search](https://www.epa.gov/enviro/tri-customized-search)
- **Tags:** Government, ToxicRelease, EnvironmentalReporting

### EPA ATTAINS Web Services

Assessment, Total Maximum Daily Load Tracking and Implementation System — REST/JSON services for state water quality assessments, impaired waters, TMDLs, and actions.

- **Base URL:** `https://attains.epa.gov/attains-public/api`
- **Documentation:** [https://www.epa.gov/waterdata/get-data-access-public-attains-data](https://www.epa.gov/waterdata/get-data-access-public-attains-data)
- **Tags:** Government, WaterQuality, Assessments

### EPA WATERS — Watershed Assessment, Tracking & Environmental Results

Geospatial water program services including StreamCat, NHDPlus, and ATTAINS overlays.

- **Base URL:** `https://watersgeo.epa.gov/openapi/waters`
- **Documentation:** [https://www.epa.gov/waterdata/waters-watershed-assessment-tracking-environmental-results-system](https://www.epa.gov/waterdata/waters-watershed-assessment-tracking-environmental-results-system)
- **Tags:** Government, WaterQuality, GIS, Watersheds

### EPA Grants API

Internal-with-key access to NGGS grant programs — applications, obligations, place of performance, and funding opportunities. GraphQL plus REST format dispatchers (JSON/XML/CSV/Excel/PDF/HTML).

- **Base URL:** `https://data.epa.gov/dmapinternalservice/query`
- **Documentation:** [https://www.epa.gov/data/grants-api](https://www.epa.gov/data/grants-api)
- **Tags:** Government, Grants, Funding

### EPA Insect Repellents API

Searchable inventory of EPA-registered insect repellent products with active ingredient, target pest, and duration data.

- **Base URL:** `https://www.epa.gov/insect-repellents`
- **Documentation:** [https://www.epa.gov/developers/data-data-products-insect-repellents-api](https://www.epa.gov/developers/data-data-products-insect-repellents-api)
- **Tags:** Government, PublicHealth, Pesticides

### EPA e-Manifest Hazardous Waste Tracking

Electronic hazardous waste manifest tracking system with REST APIs for manifest creation, retrieval, search, and lifecycle management. Production access via NAAS/CDX.

- **Base URL:** `https://rcrainfopreprod.epa.gov/rcrainfo/rest/api/v1/emanifest`
- **Documentation:** [https://github.com/USEPA/e-manifest](https://github.com/USEPA/e-manifest)
- **Tags:** Government, HazardousWaste, Manifests

### EPA System of Registries (SoR)

Authoritative registries of substances, regulatory programs, terminology, and crosswalks used across EPA systems.

- **Base URL:** `https://sor.epa.gov/sor_internet/registry`
- **Documentation:** [https://sor.epa.gov/sor_internet/registry/sysofreg/home/overview/home.do](https://sor.epa.gov/sor_internet/registry/sysofreg/home/overview/home.do)
- **Tags:** Government, Registries, MasterData

### CTX — Center for Computational Toxicology and Exposure APIs

Chemical, hazard, bioactivity, and exposure data covering tens of thousands of chemicals. Includes Chemical, Bioactivity, Hazard, Exposure, and ToxRefDB endpoints.

- **Base URL:** `https://api-ccte.epa.gov`
- **Documentation:** [https://comptox.epa.gov/ctx-api/docs/](https://comptox.epa.gov/ctx-api/docs/)
- **Tags:** Government, ChemicalSafety, Toxicology

## Common Properties

- **Website:** [https://www.epa.gov](https://www.epa.gov)
- **DeveloperPortal:** [https://www.epa.gov/developers](https://www.epa.gov/developers)
- **APIReference:** [https://www.epa.gov/data/application-programming-interface-api](https://www.epa.gov/data/application-programming-interface-api)
- **GettingStarted:** [https://www.epa.gov/data](https://www.epa.gov/data)
- **Documentation:** [https://www.epa.gov/developers/data-data-products](https://www.epa.gov/developers/data-data-products)
- **GitHubOrganization:** [https://github.com/USEPA](https://github.com/USEPA)
- **Blog:** [https://www.epa.gov/newsroom](https://www.epa.gov/newsroom)
- **YouTube:** [https://www.youtube.com/c/USEPAgov](https://www.youtube.com/c/USEPAgov)
- **X:** [https://twitter.com/EPA](https://twitter.com/EPA)
- **LinkedIn:** [https://www.linkedin.com/company/u-s--environmental-protection-agency/](https://www.linkedin.com/company/u-s--environmental-protection-agency/)
- **Support:** [https://www.epa.gov/home/forms/contact-epa](https://www.epa.gov/home/forms/contact-epa)
- **Contact:** [https://www.epa.gov/aboutepa/forms/contact-us-about-epa](https://www.epa.gov/aboutepa/forms/contact-us-about-epa)
- **PrivacyPolicy:** [https://www.epa.gov/privacy](https://www.epa.gov/privacy)
- **TermsOfService:** [https://www.epa.gov/privacy/privacy-and-security-notice](https://www.epa.gov/privacy/privacy-and-security-notice)
- **StatusPage:** [https://status.epa.gov/](https://status.epa.gov/)
- **Newsletter:** [https://www.epa.gov/newsroom/email-subscriptions-epa-news-releases](https://www.epa.gov/newsroom/email-subscriptions-epa-news-releases)
- **Compliance:** [https://echo.epa.gov/](https://echo.epa.gov/)
- **StackOverflow:** [https://stackoverflow.com/questions/tagged/epa](https://stackoverflow.com/questions/tagged/epa)
- **SpectralRules:** [rules/epa-rules.yml](rules/epa-rules.yml)
- **Vocabulary:** [vocabulary/epa-vocabulary.yml](vocabulary/epa-vocabulary.yml)
- **RateLimits:** [rate-limits/epa-rate-limits.yml](rate-limits/epa-rate-limits.yml)
- **JSONLD:** [json-ld/epa-context.jsonld](json-ld/epa-context.jsonld)
### Features

- **Open Government Data** — Most public datasets and APIs are freely accessible without authentication.
- **Cross-program Indexing** — FRS and ECHO crosswalk facilities across CAA, CWA, RCRA, SDWA, and TRI.
- **Bulk Downloads** — Annual / quarterly bulk downloads in CSV, Excel, and Parquet supplement live APIs.
- **Geospatial Layers** — WATERS, How's My Waterway, and StreamCat expose hydrography overlays.
- **State Primacy** — Many program datasets flow from state primacy agencies into national systems.
- **API Key Tiers** — Some surfaces (AQS, CAM, Grants) require email-or-portal-registered keys with documented rate limits.

### UseCases

- **Environmental Justice Analysis** — Overlay TRI, ECHO, and AQS data with demographic layers to identify cumulative impacts.
- **Compliance Screening** — Use ECHO and the Detailed Facility Report to vet sites in M&A diligence or permit reviews.
- **Air Quality Forecasting** — Combine AQS observations with NWS / EPA AirNow forecasts for public-facing apps.
- **Hazardous Waste Tracking** — Integrate the e-Manifest API into waste generator and transporter logistics systems.
- **Drinking Water Reporting** — Use SDWIS via ECHO to monitor public water system violations and inform consumer notifications.
- **Climate / Decarbonization** — Pull CAM emissions and GHGRP data for power-sector carbon analytics and FrEDI-style impact modeling.
- **Chemical Risk Assessment** — Use CTX (Chemical, Hazard, Bioactivity, Exposure) data plus ToxCast/ToxRefDB to triage substances.
- **Watershed Restoration** — Combine ATTAINS impairments, How's My Waterway, and StreamCat metrics for restoration planning.

### Integrations

- **api.data.gov** — Government-wide API management front-door for several EPA APIs with X-API-Key sign-up flow.
- **data.gov** — Federal open data catalog cross-listing every EPA-published dataset.
- **NAAS / CDX** — EPA's Network Authentication & Authorization Services for credentialed submissions (FRS Submit, e-Manifest, NEI).
- **State Environmental Agencies** — State primacy programs forward data into AQS, ECHO, SDWIS, RCRAInfo, and TRI.
- **USGS, NOAA, USDA** — Cross-agency data sharing for water, weather, and agricultural environmental data.

### Solutions

- **Public-Facing Awareness** — How's My Waterway, AirNow, and Insect Repellents are designed for consumer use.
- **Regulatory Compliance** — ECHO, RCRAInfo, NPDES eDMR, e-Manifest support regulated-entity reporting workflows.
- **Scientific Research** — CTX, ToxCast, ToxRefDB, EPA HTTK, FrEDI underpin chemical safety and climate research.
- **Internal Government** — FRS Submit, SoR, Grants, CSB Rebate APIs support EPA program operations and grantees.


## Maintainers
- **Kin Lane** — kin@apievangelist.com
