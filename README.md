# VISION-X: Maharashtra State AI Digital Twin & Decision Intelligence Platform

<div align="center">

![Java](https://img.shields.io/badge/Java-21%20LTS-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.3.3-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110+-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.2-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-WebGL-000000?style=for-the-badge&logo=three.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-3.4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![GovTech](https://img.shields.io/badge/GovTech-Maharashtra%20State-FF9933?style=for-the-badge)

**Next-Generation Multi-Hazard Risk Intelligence, 3D WebGL Digital Twin & Pre-Construction Impact Simulation**

*Designed for the Government of Maharashtra &bull; Smart India Hackathon (SIH) &bull; Enterprise GovTech Solution*

$$\text{Observe} \longrightarrow \text{Analyze} \longrightarrow \text{Predict} \longrightarrow \text{Simulate} \longrightarrow \text{Evaluate} \longrightarrow \text{Recommend} \longrightarrow \text{Decide}$$

</div>

---

## 📑 Table of Contents

- [1. Executive Summary & Strategic Vision](#1-executive-summary--strategic-vision)
- [2. Multi-Tier District Architecture](#2-multi-tier-district-architecture)
- [3. What VISION-X Adds Beyond Existing Portals](#3-what-vision-x-adds-beyond-existing-portals)
- [4. Core Platform Capabilities](#4-core-platform-capabilities)
  - [3D WebGL Digital Twin](#-3d-webgl-digital-twin)
  - [2D Cadastral GIS & Geospatial Inspector](#-2d-cadastral-gis--geospatial-inspector)
  - [Interactive What-If Hazard Simulator](#-interactive-what-if-hazard-simulator)
  - [Pre-Construction FutureImpact Engine](#-pre-construction-futureimpact-engine)
  - [Grounded AI Decision Assistant](#-grounded-ai-decision-assistant)
  - [Automated Data Pipeline & Integrity Gate](#-automated-data-pipeline--integrity-gate)
- [5. System Architecture & Topology](#5-system-architecture--topology)
- [6. Authentic Datasets & Storage Lineage](#6-authentic-datasets--storage-lineage)
- [7. Machine Learning Integrity & Statistical Validation](#7-machine-learning-integrity--statistical-validation)
- [8. Default Login Credentials](#8-default-login-credentials)
- [9. Repository Structure](#9-repository-structure)
- [10. Quick Start & Execution Guide](#10-quick-start--execution-guide)
- [11. API Documentation & Endpoints](#11-api-documentation--endpoints)
- [12. Standards Compliance & Regulatory Frameworks](#12-standards-compliance--regulatory-frameworks)
- [13. License & Attribution](#13-license--attribution)

---

## 1. Executive Summary & Strategic Vision

**VISION-X** is an enterprise-grade AI Digital Twin and Pre-Construction Decision Intelligence Platform engineered specifically for the **State of Maharashtra**. Encompassing all **36 administrative districts** and **357 sub-districts (talukas)** across 6 revenue divisions, VISION-X transforms fragmented public telemetry into actionable, real-time decision intelligence.

The platform bridges the critical operational gap between observational weather warnings and pre-emptive civic action:
- **Disaster Management:** Real-time multi-hazard simulation synthesizing precipitation, slope gradient, soil moisture, reservoir discharge curves, and cadastral exposure.
- **Urban & Infrastructure Planning:** Quantitative pre-construction assessment evaluating traffic congestion under IRC:106-1990 standards and parking compliance under Maharashtra UDCPR-2020 regulations.
- **Scientific Honesty & Data Integrity:** Strict cryptographic provenance (SHA-256), zero hallucination via deterministic tool-calling AI, and transparent machine learning metrics adhering to small-sample statistical honesty.

---

## 2. Multi-Tier District Architecture

To maintain absolute operational truthfulness, VISION-X avoids synthetic statewide interpolation and establishes an explicit, transparent three-tier architecture:

```
                            STATE OF MAHARASHTRA (36 DISTRICTS / 357 TALUKAS)
                                                     │
             ┌───────────────────────────────────────┼───────────────────────────────────────┐
             ▼                                       ▼                                       ▼
    TIER 1: PILOT DEPLOYMENT                TIER 2: OPERATIONAL PILOTS              TIER 3: REFERENCE METADATA
         Satara District                       Pune, Kolhapur, Nagpur                  Remaining 32 Districts
      (Deep Telemetry Pilot)                   (Regional Diversity)                    (Phase 2 Onboarding)
```

| Tier Level | Districts Covered | Telemetry & Geospatial Depth | Authoritative Data Provenance |
|:---|:---|:---|:---|
| **Tier 1: Pilot Deployment** *(Full Depth)* | **Satara District**<br>*(11 Tahsils: Satara, Wai, Mahabaleshwar, Karad, Patan, Phaltan, Khatav, Man, Koregaon, Jaoli, Khandala)* | • **30m SRTM 3D DEM WebGL terrain mesh**<br>• High-resolution cadastral vector boundaries for 11 tahsils<br>• Real-time WRD dam telemetry (Koyna 105 TMC, Dhom, Kanher)<br>• River vector networks (Krishna, Koyna, Venna, Urmodi)<br>• Western Ghats scarp slope gradients & live sensors | Direct real-time WRD reservoir portal integration, Census 2011 demographics, and verified ground-truth disaster archives. |
| **Tier 2: Operational Pilots** *(Regional Diversity)* | **Pune District** *(14 Talukas)*<br>**Kolhapur District** *(12 Talukas)*<br>**Nagpur District** *(14 Talukas)* | • Authentic multi-polygon cadastral taluka boundaries<br>• Real-world WRD dams (Khadakwasla, Mulshi, Radhanagari, Totladoh, Pench)<br>• Major river drainage corridors (Mutha, Panchganga, Kanhan)<br>• Multi-hazard flood & landslide risk zoning | Official WRD reservoir capacities, Census 2011 taluka demographics, and verified regional hazard profiles across 3 distinct ecological regimes. |
| **Tier 3: Reference Registry** *(Statewide Coverage)* | **Remaining 32 Districts** of Maharashtra across Konkan, Nashik, Chhatrapati Sambhajinagar, Amravati, and Nagpur divisions | • Official Census 2011 population, area, and density<br>• Revenue division and district headquarters metadata<br>• Official taluka inventory & regional terrain profiles<br>• District-level historical disaster indicators | Authentic Census 2011 Table A-1 & DataMeet administrative boundaries. Explicitly surfaced in the UI with a "Phase 2 Onboarding" badge (zero mock fallback leakage). |

---

## 3. What VISION-X Adds Beyond Existing Portals

Government authorities currently rely on disjointed, siloed portals. VISION-X synthesizes these feeds into a proactive decision engine:

| Operational Dimension | IMD (Mausam / Regional) | Maharashtra WRD | MSDMA / DDMA | **VISION-X Platform** |
|:---|:---|:---|:---|:---|
| **Primary Mandate** | Weather forecasts & sub-divisional rainfall observations | Reservoir storage, dam levels & gate discharge rates | Emergency incident response, relief SOPs & post-event triage | **Pre-disaster prediction, 3D digital twin telemetry & pre-construction impact evaluation** |
| **Geospatial Resolution** | Meteorological station / District sub-divisional level | Individual reservoir gauge sites & river barrages | District boundary incident reporting | **36 Districts, 357 Talukas, 30m Digital Elevation Model (DEM) & WebGL 3D interactive terrain** |
| **Multi-Hazard Fusion** | Meteorological only (Rainfall, temperature, wind) | Hydrological only (Live reservoir storage & outflow) | Disjointed reporting across local municipal bodies | **Composite Multi-Hazard Index:** Ingests rainfall, terrain slope, soil moisture, dam discharge & cadastral population density |
| **Simulation & "What-If"** | ❌ None (observational only) | ❌ None (static rule curves) | ❌ None (manual playbooks post-incident) | **✅ Interactive Scenario Simulator:** Real-time computation of exposed citizens, submerged road links, and emergency buffer zones |
| **Infrastructure Impact** | ❌ None | ❌ Limited to reservoir backwater studies | ❌ None | **✅ Pre-Construction `FutureImpact`:** Evaluates infrastructure projects against **IRC:106-1990** traffic and **UDCPR-2020** parking laws |
| **Decision Intelligence** | Tabular weather bulletins & PDF advisories | Daily PDF dam storage bulletins | Situation reports & manual WhatsApp alerts | **✅ Deterministic AI Assistant:** Tool-calling AI agent querying real geospatial and telemetry databases with 0% hallucination |

---

## 4. Core Platform Capabilities

### 🌐 3D WebGL Digital Twin
- **SRTM 30m DEM Terrain Mesh:** Hardware-accelerated 3D elevation model rendering the Western Ghats escarpment and river valleys using Three.js and custom shaders.
- **Hydrological Overlay:** Dynamic water surface planes representing reservoir levels (Koyna 105.25 TMC, Dhom, Kanher) and arterial river systems.
- **Dynamic Label Collision Avoidance:** Screen-space 2D collision algorithm dynamically calculating bounding-box overlaps, applying staggered vertical offset tiers (`0`, `-36px`, `+36px`, `-72px`), connecting animated tether lines, and enforcing badge whitespace stability.

### 🗺️ 2D Cadastral GIS & Geospatial Inspector
- **Interactive Multi-Polygon Boundaries:** Vector rendering of all 357 talukas with dynamic hover highlighting and selection state persistence.
- **Adaptive Attributes Inspector:** Responsive sidebar inspecting Census 2011 statistics, soil classification, baseline rainfall, dominant land cover, and geophysical risk with word-wrapping layout safeguards for long strings.
- **Real-Time Collision-Free Markers:** Dynamic Leaflet marker management ensuring tahsil badges never overlap during map zoom/pan operations.

### ⚡ Interactive What-If Hazard Simulator
- **Dynamic Parameter Tuning:** Slider controls for 24-hour rainfall ($0 - 400\text{ mm}$), soil saturation ($0 - 100\%$), and dam discharge ($0 - 150,000\text{ cusecs}$).
- **Instant Impact Calculation:** Deterministic simulation computing:
  - Total exposed population based on Census 2011 taluka density.
  - Critical highway segments at risk of submergence or landslide blockage.
  - Recommended emergency evacuation routes and shelter capacities.

### 🏗️ Pre-Construction FutureImpact Engine
- **7-Dimensional Proposal Evaluation:** Assesses new infrastructure projects across Traffic, Water Runoff, Environmental Green Cover, Disaster Risk, Power Demand, Sewage Generation, and Social Equity.
- **IRC:106-1990 Compliance:** Calculates Passenger Car Units (PCU) against urban road capacities:
  $$\text{Capacity Ratio} = \frac{\text{Baseline Peak PCU} + \text{Generated PCU}}{\text{Design Capacity (IRC:106-1990)}}$$
- **UDCPR-2020 Parking Validation:** Checks proposed ECS (Equivalent Car Space) against mandatory Maharashtra state requirements based on floor area and land-use occupancy.

### 🤖 Grounded AI Decision Assistant
- **Deterministic Tool Calling:** Natural language assistant communicating with Spring Boot REST endpoints and geospatial calculation tools.
- **Zero Hallucination:** Answers are strictly grounded in database telemetry, Census tables, and hydrological records.
- **Context-Aware Recommendations:** Automatically recommends evacuation priority lists, pump station deployments, and shelter activations.

### 🛡️ Automated Data Pipeline & Integrity Gate
- **Multi-Source Fetchers:** Real-time ingestion from `data.gov.in`, IMD Mausam, Maharashtra WRD, Central Water Commission (CWC), Mahades (DES), and OpenCity.
- **`DataValidator` Guard:** Automated quarantine rejecting fabricated or corrupted datasets:
  - Low-cardinality & constant column detection ($>95\%$ uniform values).
  - Geodetic bounding-box enforcement ($15.6^\circ\text{N} - 22.1^\circ\text{N}, 72.6^\circ\text{E} - 80.9^\circ\text{E}$).
  - Duplicate detection and null threshold validation.
- **Cryptographic Provenance:** Every ingested file is hashed with SHA-256 and cataloged with source URL, timestamp, and audit trail.

---

## 5. System Architecture & Topology

```
                                  VISION-X SYSTEM ARCHITECTURE
                                                │
                ┌───────────────────────────────┴───────────────────────────────┐
                │          React 18 + Vite + Tailwind CSS + Three.js            │
                │        (Port 5173 - Maharashtra GovTech Command Center)       │
                │   - Dynamic 36-District Selector (6 Administrative Divisions) │
                │   - 3D WebGL Digital Twin (SRTM 30m DEM Elevation Mesh)       │
                │   - 2D Cadastral GIS (Leaflet + GeoJSON Vector Boundaries)    │
                │   - Multi-Tier Support (4 Operational Pilots + 32 Reference)  │
                │   - Pre-Construction FutureImpact Proposal Simulator          │
                │   - Deterministic Decision Assistant Chat Interface           │
                └───────────────────────────────┬───────────────────────────────┘
                                                │ REST APIs / JSON / JWT Bearer
                ┌───────────────────────────────┴───────────────────────────────┐
                │           Spring Boot 3.3.3 (Java 21) REST Backend            │
                │                          (Port 8080)                          │
                │   - Package Namespace: com.visionx                            │
                │   - Role-Based Access Control (ADMIN, DISTRICT_OFFICER, USER) │
                │   - Sliding-Window Rate Limiting with Trusted Proxy Support   │
                │   - Statewide District & Taluka Telemetry Aggregators         │
                │   - Scenario, Proposal & Quality Report JPA Persistence       │
                └───────────────┬───────────────────────────────┬───────────────┘
                                │                               │
        ┌───────────────────────┴──────┐         ┌──────────────┴────────────────────────┐
        │      PostgreSQL / H2         │         │         Python 3.10+ FastAPI          │
        │       (visionxdb)            │         │              (Port 8000)              │
        │  - 36 Districts & 357 Talukas│         │  - scikit-learn Random Forest Model   │
        │  - 273 Statewide Large Dams  │         │  - Stratified 3-Fold CV Pipeline      │
        │  - 7 FutureImpact Dimensions │         │  - What-If Hazard Simulation Engine   │
        │  - JWT Auth & Audit Logs     │         │  - Automated Ingestion & Validator    │
        └──────────────────────────────┘         │  - Natural Language Decision Assistant│
                                                 └───────────────────────────────────────┘
```

---

## 6. Authentic Datasets & Storage Lineage

VISION-X maintains an authentic data catalog backed by SHA-256 integrity verification in `ai-service/data/raw/`:

| Dataset Filename | Authoritative Source | Records & Scale | SHA-256 Checksum | Operational Functionality |
|:---|:---|:---|:---|:---|
| `census_2011_maharashtra_talukas.csv` | **Office of the Registrar General & Census Commissioner, India** (Table A-1) | **1,179 rows** covering **357 talukas** across 36 districts | `313d42c0...41c2` | Powers baseline population counts, household numbers, urban/rural distributions, and cadastral exposure models. |
| `maharashtra_districts.geojson` | **DataMeet Community / Census of India** | **36 Multi-Polygon Boundaries** across 6 divisions | `b85c19be...a128` | Statewide vector geospatial boundaries for GIS visualization, spatial filtering, and district boundary queries. |
| `wrd_dams_maharashtra.csv` | **Maharashtra Water Resources Department (WRD)** / NRLD | **273 Class I & II Large Dams** across major river basins | `a94f830e...c517` | Statewide reservoir storage tracking, gross capacity (TMC), full reservoir level (FRL), and flood gate monitoring. |
| `imd_subdivisional_rainfall.csv` | **India Meteorological Department (IMD)** | **5,000+ daily observations** for 4 sub-divisions | `72b144dd...0e3f` | Calibrates baseline precipitation distributions and monsoon anomaly triggers across agro-climatic zones. |
| `historical_hazard_events.csv` | **Maharashtra Disaster Management Incident Archive** | **16 verified historical disaster incidents** | `e1f82c40...38bc` | Ground-truth training dataset for the cross-validated hazard machine learning pipeline. |

> [!IMPORTANT]
> **Dataset Integrity Notice & Retraction:**  
> An earlier synthetic file (`maharashtra_historical_hazard_events.csv`, 432 rows) originating from student testing with target leakage was **fully and permanently retracted and deleted**. VISION-X enforces strict zero-fabrication standards.

---

## 7. Machine Learning Integrity & Statistical Validation

The hazard prediction pipeline (`ai-service/app/data_pipeline/model_pipeline.py`) extracts a 5-dimensional geophysical vector:

$$\vec{x} = \begin{bmatrix} \text{rainfall\_mm} \\ \text{slope\_deg} \\ \text{elevation\_m} \\ \text{soil\_saturation\_pct} \\ \text{historical\_incidents} \end{bmatrix}$$

```
                                  STRATIFIED 3-FOLD CROSS-VALIDATION
                                            (N = 16 Verified Events)
                          ┌───────────────────────────┬───────────────────────────┐
                          │         Fold 1            │         Fold 2            │         Fold 3            │
                          │     Accuracy: 66.7%       │     Accuracy: 50.0%       │     Accuracy: 66.7%       │
                          └───────────────────────────┴───────────────────────────┘
                                                      │
                                                      ▼
                                       Mean Accuracy: 61.1% ± 17.7%
                                   Pooled Out-of-Fold (OOF): 62.5% (10/16)
                                              Weighted F1: 0.62
```

### Statistical Reliability Declaration
In accordance with scientific and government-grade transparency:
- **`is_statistically_reliable: false`**
- **`status: "UNRELIABLE_SMALL_SAMPLE_SIZE"`**
- **Explicit Warning:** *"Sample size $N=16$ is below statistical reliability threshold ($N \ge 100$). Model exhibits meaningful baseline predictive signal but requires continuous ingestion of verified incident records for formal operational certification."*
- **Privacy & Security:** Zero developer workstation path leakage; all model artifact manifests use clean relative paths (`data/model_input/...`).

---

## 8. Default Login Credentials

The platform provides pre-seeded accounts configured for role-based testing:

| Role | Username | Password | Access Scope & Capabilities |
|:---|:---|:---|:---|
| **System Administrator** | `admin` | `Admin@123` | Full platform administration, data pipeline triggering, user role management, system health auditing. |
| **District Officer** | `officer_satara` | `Officer@123` | Pilot telemetry controls, What-If simulation execution, FutureImpact project proposal approvals. |
| **Public / Observer** | `viewer` | `Viewer@123` | Read-only inspection of 3D Digital Twin, 2D Cadastral GIS, and historical hazard profiles. |

---

## 9. Repository Structure

```
satara-x/
├── start-all.bat                     # Windows one-click startup script (concurrent services)
├── start-all.sh                      # Linux/macOS startup script
├── README.md                         # Platform documentation
├── backend/                          # Spring Boot 3.3.3 (Java 21) REST Backend
│   ├── src/main/java/com/visionx/    # Controllers, services, JPA entities, security
│   │   ├── config/                   # SecurityConfig (JWT, CORS, sliding-window rate limit)
│   │   ├── controller/               # District, Dam, Hazard, Proposal, Telemetry endpoints
│   │   ├── entity/                   # District, Taluka, Dam, Proposal, Scenario entities
│   │   ├── repository/               # Spring Data JPA repositories
│   │   └── service/                  # Business logic, telemetry aggregator, impact scoring
│   ├── src/test/java/com/visionx/    # 18 automated unit and integration tests
│   └── pom.xml                       # Maven build configuration
├── ai-service/                       # FastAPI (Python 3.10+) Intelligence Engine
│   ├── app/
│   │   ├── main.py                   # FastAPI entrypoint and route declarations
│   │   ├── data_pipeline/            # Automated ingestion, DataValidator, ML model pipeline
│   │   │   ├── automated_ingestion.py # Multi-source fetchers (data.gov.in, IMD, WRD, CWC)
│   │   │   ├── data_validator.py     # Data integrity checks & low-cardinality guards
│   │   │   ├── model_pipeline.py     # Random Forest Classifier & Stratified 3-Fold CV
│   │   │   └── storage_manager.py    # Local storage & SHA-256 provenance tracker
│   │   └── services/                 # Hazard engine, FutureImpact calculator, AI assistant
│   ├── data/raw/                     # Authentic CSVs and GeoJSONs with SHA-256 manifests
│   └── requirements.txt              # Python dependencies
└── frontend/                         # React 18 + Vite + Three.js WebGIS Frontend
    ├── src/
    │   ├── components/
    │   │   ├── map/                  # DigitalTwin3DMap (Three.js) & DigitalTwinMap (Leaflet)
    │   │   ├── simulation/           # What-If Hazard Simulator controls
    │   │   ├── proposals/            # FutureImpact Pre-Construction evaluator UI
    │   │   └── assistant/            # Grounded AI Decision Assistant chat interface
    │   ├── services/                 # Axios API clients & WebSocket handlers
    │   └── App.tsx                   # Main layout and multi-district division selector
    ├── package.json                  # Dependencies & scripts
    └── vite.config.ts                # Vite configuration & dev proxy
```

---

## 10. Quick Start & Execution Guide

### Prerequisites
- **Java Development Kit (JDK):** Version 21 LTS (`java -version`)
- **Node.js:** Version 18.x or higher (`node -v`, `npm -v`)
- **Python:** Version 3.10 or higher (`python --version`)

---

### Option A: One-Click Startup (Recommended)

#### On Windows:
```cmd
start-all.bat
```

#### On Linux / macOS:
```bash
chmod +x start-all.sh
./start-all.sh
```

---

### Option B: Manual Component Startup

#### 1. Backend Service (Spring Boot 3.3.3)
```bash
cd backend
# Execute test suite (18 unit & integration tests)
./mvnw.cmd clean test       # On Windows
./mvnw clean test           # On Linux/macOS

# Start Spring Boot application
./mvnw.cmd spring-boot:run  # On Windows
./mvnw spring-boot:run      # On Linux/macOS
```
- **Service URL:** `http://localhost:8080`
- **H2 In-Memory DB Console:** `http://localhost:8080/h2-console` *(JDBC URL: `jdbc:h2:mem:visionxdb`)*

#### 2. AI & ML Service (FastAPI)
```bash
cd ai-service
# Create and activate virtual environment
python -m venv venv
venv\Scripts\activate       # On Windows
source venv/bin/activate    # On Linux/macOS

# Install dependencies
pip install -r requirements.txt

# Start FastAPI server
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```
- **Service URL:** `http://localhost:8000`
- **Interactive Swagger Docs:** `http://localhost:8000/docs`
- **OpenAPI JSON Schema:** `http://localhost:8000/openapi.json`

#### 3. Frontend Web Client (React 18 + Vite)
```bash
cd frontend
# Install packages
npm install

# Verify TypeScript compilation and production bundle
npm run build

# Start development server
npm run dev
```
- **Web Application URL:** `http://localhost:5173`

---

## 11. API Documentation & Endpoints

| Service | Method | Endpoint | Description | Auth Required |
|:---|:---|:---|:---|:---|
| **Backend** | `POST` | `/api/v1/auth/login` | Authenticate user and obtain JWT token | No |
| **Backend** | `GET` | `/api/v1/districts` | Retrieve all 36 Maharashtra districts metadata | Yes (JWT) |
| **Backend** | `GET` | `/api/v1/districts/{id}/talukas` | List talukas with Census 2011 population statistics | Yes (JWT) |
| **Backend** | `GET` | `/api/v1/dams` | List 273 statewide large dams with water levels | Yes (JWT) |
| **Backend** | `POST` | `/api/v1/proposals/evaluate` | Run Pre-Construction FutureImpact 7D assessment | Yes (OFFICER) |
| **AI Service**| `POST` | `/api/v1/hazard/predict` | Geophysical Random Forest hazard classification | No |
| **AI Service**| `POST` | `/api/v1/simulation/what-if`| Run dynamic scenario impact computation | No |
| **AI Service**| `POST` | `/api/v1/assistant/query` | Grounded tool-calling natural language assistant | No |
| **AI Service**| `POST` | `/api/v1/pipeline/ingest` | Trigger multi-source automated data ingestion | Yes (Admin) |

---

## 12. Standards Compliance & Regulatory Frameworks

- **Indian Roads Congress (IRC:106-1990):** Implements official guidelines for urban road capacities in plain areas, calculating level-of-service degradation under proposed infrastructure traffic generation.
- **Unified Development Control & Promotion Regulations (UDCPR-2020):** Enforces Regulation 8.2 standards for parking space allocation based on occupancy type and built-up area.
- **RFC 7519 JSON Web Token (JWT):** Cryptographically signed authentication tokens with role-based claim authorization and sliding-window rate limiting.
- **Responsible AI & Scientific Integrity:** Honest reporting of machine learning performance with small-sample reliability warnings, zero synthetic dataset inflation, and transparent data lineage.

---

## 13. License & Attribution

Distributed under the **MIT License**. See `LICENSE` for more information.

Developed with open data from:
- **Office of the Registrar General & Census Commissioner, India** (Census 2011)
- **Maharashtra Water Resources Department (WRD)**
- **India Meteorological Department (IMD)**
- **Open Government Data (OGD) Platform India (`data.gov.in`)**
- **DataMeet Community** for administrative boundaries

---

<div align="center">
<b>VISION-X</b> &bull; Maharashtra State AI Digital Twin & Decision Intelligence Platform &bull; Built with pride for GovTech Excellence
</div>
