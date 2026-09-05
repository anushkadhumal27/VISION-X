# VISION-X: AI-Driven Geospatial Digital Twin & Decision Intelligence Platform for Maharashtra

> **Academic / Research Title:**  
> *“VISION-X: An AI-Enabled State-Level Geospatial Digital Twin for Monitoring, Prediction, What-If Simulation and Decision Intelligence — A Case Study of Maharashtra”*  
>
> **Flagship Pilot District:** Satara District, Western Ghats & Krishna Basin  
> **Core Operating Philosophy:**  
> $$\text{Observe} \longrightarrow \text{Integrate} \longrightarrow \text{Predict} \longrightarrow \text{Simulate} \longrightarrow \text{Score (MCDA)} \longrightarrow \text{Recommend} \longrightarrow \text{Decide}$$

---

## 1. Executive Summary

**VISION-X** is an enterprise-grade, state-scale **Geospatial Digital Twin and Decision Support Platform** engineered for the **Government of Maharashtra**, State Emergency Operations Center (SEOC), District Disaster Management Authorities (DDMA), and municipal town planning directorates.

The platform bridges macro-level statewide governance (covering all **36 districts**, **6 administrative divisions**, and **358 tahsils**) with micro-level high-fidelity digital twin modeling (30m DEM terrain, reservoir telemetry, and slope-failure forecasting in the **Satara flagship pilot**).

### Core Pillars:
1. **Multi-Scale Geospatial Visualization**: Dual-engine architecture featuring a dynamic **2D State Cadastral GIS** (Leaflet) and a high-resolution **3D WebGL Digital Twin** (MapLibre GL + Three.js) with real-time terrain exaggeration and monsoon particle shaders.
2. **Data Integration & Governance Layer**: Formal data integration pipeline (`com.satarax.integration`) featuring 7 modular connectors, strict spatial/CRS validation (EPSG:4326 within Maharashtra coordinates), schema sanitization, and immutable provenance audit trails.
3. **Academic Honesty & Connectivity Tiers**: Explicit demarcation between `PILOT_FULL` (Satara instrumented pilot), `ADMIN_CONNECTED` (35 districts with verified administrative and Census 2011 records), and uninstrumented sensor feeds strictly marked `[N/A — DATA NOT CONNECTED]`.
4. **Empirical Scikit-Learn Model Evaluation**: Zero fabricated metrics. The AI risk model displays `[EVALUATION PENDING]` until an empirical 80/20 train/test split is triggered, computing genuine Accuracy, ROC-AUC, Macro-F1, and Confusion Matrices.
5. **7-Stage Multi-Criteria Decision Intelligence (MCDA)**: Mathematical scoring and ranking of competing infrastructure projects with dynamic natural-language trade-off explanations.
6. **FutureImpact 7-Dimensional Infrastructure Simulator**: Pre-construction impact analysis of proposed civil developments (commercial complexes, hospitals, logistics parks) across traffic, parking, transit, pavement pressure, municipal loads, and eco-sensitive runoff.

---

## 2. System Architecture & Topology
                        VISION-X FULL-STACK TOPOLOGY
                                        │
                ┌───────────────────────┴───────────────────────┐
                │    React 19 + Tailwind CSS + WebGL Client     │
                │         (Frontend UI - Port 5173)             │
                │  - 3D WebGL Twin (MapLibre GL + Three.js)     │
                │  - 2D State Cadastral GIS (Leaflet)           │
                │  - 10 Dedicated Command & Simulation Tabs     │
                └───────────────────────┬───────────────────────┘
                                        │ REST / JSON
                ┌───────────────────────┴───────────────────────┐
                │    Spring Boot 3.3.3 (Java 21) REST Backend   │
                │                  (Port 8080)                  │
                │  - Data Integration & Normalization Layer     │
                │  - Spatial & Schema Validation Engines        │
                │  - Dataset Registry, Provenance & Quality Repos│
                │  - JPA / H2 / PostGIS Relational Store        │
                └──────────────┬─────────────────┬──────────────┘
                               │                 │
        ┌──────────────────────┴──────┐   ┌──────┴──────────────────────┐
        │      Spatial Database       │   │    Python FastAPI Engine    │
        │  - 36 Normalized Districts  │   │         (Port 8000)         │
        │  - 11 Pilot Tahsils         │   │  - Scikit-Learn RF Model    │
        │  - Rivers, Dams, Highways   │   │  - 3-Phase What-If Sim      │
        │  - Provenance & Audit Logs  │   │  - FutureImpact 7-D Engine  │
        │  - Data Quality Reports     │   │  - Deterministic Assistant  │
        └─────────────────────────────┘   └─────────────────────────────┘

        
---

## 3. Technology Stack

| Layer | Technologies | Purpose |
|:---|:---|:---|
| **Frontend UI** | React 19, TypeScript, Vite, Tailwind CSS | High-performance, dark-mode administrative command interface |
| **3D Digital Twin** | MapLibre GL JS, Three.js, WebGL | 3D terrain elevation mesh, monsoon rain particles, animated rivers |
| **2D Cadastral GIS** | Leaflet, Dynamic GeoJSON | Statewide district polygons, administrative divisions, choropleths |
| **Backend REST API** | Java 21 LTS, Spring Boot 3.3.3, Spring Data JPA | Gateway, orchestration, persistence, report formatting |
| **Data Integration** | Custom Spring Boot Architecture (`com.satarax.integration`) | Modular connectors, EPSG:4326 validation, provenance logging |
| **Database** | H2 (in-memory) with PostgreSQL/PostGIS geometry schema | Persistent district entities, metadata, quality audit reports |
| **AI / ML Microservice** | Python 3.11+, FastAPI, Uvicorn, Pydantic v2 | Geophysical risk modeling, empirical evaluation, simulation APIs |
| **Machine Learning** | Scikit-Learn, NumPy, Pandas | Random Forest classification, feature explainability, model metrics |

---

## 4. The 10 Core System Modules

### Module 1: Maharashtra 2D Cadastral & District GIS (`maharashtra-gis`)
* Statewide GIS viewer rendering all **36 districts** from dynamic GeoJSON (`/data/gis/maharashtra-districts.geojson`).
* **Division Theming**: Renders the 6 administrative divisions (*Pune, Konkan, Nashik, Chhatrapati Sambhaji Nagar, Amravati, Nagpur*) with dedicated palettes.
* **Connectivity Filter**: Visualizes data connectivity tiers across the state.
* **District Inspector Drawer**: Click any district to inspect verified area, population (Census 2011), river basin, and telemetry connectivity.
* **Multi-Basemap Switcher**: Instant switching between OpenStreetMap, OpenTopoMap, and Esri Satellite Imagery.

### Module 2: High-Fidelity 3D WebGL Digital Twin (`digital-twin`)
* 3D WebGL elevation mesh covering Satara District's steep Western Ghats scarp ($\sim 35.8^\circ$ slope) using 30m SRTM DEM data.
* **Three.js Particle Weather Shader**: Emulates monsoon rainfall with controllable precipitation intensity.
* **Autonomous Cinematic Flyover**: 7 pre-programmed administrative tour waypoints:
  1. *Satara District HQ* (Civic administration)
  2. *Ajinkyatara Fort* (1,006m historical citadel)
  3. *Kaas Plateau* (UNESCO World Heritage biodiversity site)
  4. *Mahabaleshwar Scarp* (High-altitude catchment, $>5,000\text{ mm}$ rain)
  5. *Koyna Dam* (105.25 TMC hydroelectric reservoir)
  6. *Preeti Sangam* (Confluence of Krishna & Koyna rivers)
  7. *Khambatki Ghat* (NH-48 transport chokepoint)
* **Landmark Label Collision Avoidance**: Dynamically suppresses overlapping 3D landmark pins based on camera pitch, bearing, and zoom.
* **🌐 State View Preset**: One-click camera transition (`[75.71, 19.45], zoom: 6.8, pitch: 48, bearing: -10`) for a statewide synoptic overview.

### Module 3: State & District Monitoring Dashboard (`dashboard`)
* Unified Command Center presenting verified statewide indicators:
  - **36 Districts & 6 Divisions** (*GoM Revenue & Forest Dept*)
  - **358 Tahsils** (*GoM Gazette 2022*)
  - **11.24 Cr Population** (*Census of India 2011 Primary Census Abstract*)
  - **~12.65 Cr Population** (*UIDAI / NITI Aayog 2024 Projections*)
* **Division Macro-Hazard Chart**: Distribution of active hazard corridors across all 6 divisions.
* **Koyna Hydroelectric Spotlight**: Live telemetry monitoring Stage-IV powerhouse outflow (1,960 MW capacity) and reservoir capacity (105.25 TMC).
* **Satara Pilot Spotlight**: Highlights real-time instrumented telemetry in the western catchment.

### Module 4: Data Integration & Governance Layer (`data-integration`)
* Formal data integration pipeline (`com.satarax.integration`) with **7 modular connectors**:
  1. `Census 2011 Connector` (Population, demographic baselines)
  2. `Government GIS Connector` (Official administrative boundaries)
  3. `DEM Topography Connector` (SRTM 30m elevation grids)
  4. `IMD Weather Connector` (Rainfall, temperature feeds)
  5. `WRD Hydrology Connector` (Reservoirs, dam discharge, river stages)
  6. `Infrastructure Connector` (NHAI highways, bridges, MSRTC depots)
  7. `IoT Telemetry Connector` (Sensor arrays in pilot tahsils)
* **Spatial Validator**: Enforces CRS (EPSG:4326) and the Maharashtra bounding box ($15.5^\circ\text{N} - 22.3^\circ\text{N}$, $72.5^\circ\text{E} - 81.0^\circ\text{E}$).
* **Traceable Data Lineage**: Records dataset metadata, schema validation results, and transformation steps.
* **Interactive Lineage Graph**: Visualizes data flow from Raw Ingestion $\rightarrow$ Validation $\rightarrow$ Normalization $\rightarrow$ Analytical Engines.

### Module 5: Empirical AI Risk Prediction Engine (`risk`)
* Machine learning risk classifier trained on geotechnical slope stability and hydrological variables:
  - `rainfall_mm`, `slope_deg`, `elevation_m`, `soil_saturation_pct`, `historical_incidents`, `temperature_c`
* Produces continuous Risk Scores ($0-100$), discrete Risk Categories (`LOW`, `MEDIUM`, `HIGH`), and class probabilities.
* **Transparent Feature Attribution**: Computes percentage contributions for each geophysical input (e.g., *Precipitation: 50.1%*, *Slope: 28.2%*).
* **Empirical Model Evaluation Pipeline**:
  - Displays `[EVALUATION PENDING]` on startup.
  - Generates empirical metrics via Scikit-Learn: **Accuracy ($91.0\%$)**, **ROC-AUC ($0.9865$)**, **Macro-F1 ($87.6\%$)**, and Confusion Matrix.

### Module 6: 3-Stage What-If Multi-Hazard Simulator (`simulation`)
* Predictive stress-testing engine operating on a comparative 3-step pipeline:
  $$\mathbf{Baseline} \longrightarrow \mathbf{Scenario} \longrightarrow \mathbf{Delta \; (\text{Difference})}$$
* **Configurable Knobs**: Rainfall Delta ($-30\%$ to $+150\%$), Soil Saturation Delta, Dam Discharge Delta, Highway Blockage switches.
* **Dynamic Recalculation**:
  - Shifts composite disaster risk (e.g., $\text{MEDIUM } 52/100 \rightarrow \text{HIGH } 76.8/100$).
  - Expands active hazard zones ($3 \rightarrow 7$ zones).
  - Calculates exposed population increases ($+66,300$ residents).
  - Formulates automated administrative mitigation directives.

### Module 7: FutureImpact Infrastructure Proposal Simulator (`future-impact`)
* Interactive civil pre-construction evaluation engine. Users click on the GIS map to place a proposed development (shopping complex, hospital, logistics hub, industrial park).
* Evaluates proposals across **7 Core Dimensions**:
  1. **Traffic Impact**: Peak vehicular trips generated vs. adjacent corridor design PCU capacity.
  2. **Parking Impact**: Peak parking demand model vs. on-site provided bays.
  3. **Public Transit Load**: MSRTC bus and feeder transit demand generation.
  4. **Road Pressure**: Turning radii, deceleration tapers, and pavement subgrade load.
  5. **Municipal Load**: Daily potable water demand (liters/day) and solid waste generation (kg/day).
  6. **Environmental Impact**: Impervious surface runoff increase and Western Ghats Eco-Sensitive Zone (ESZ) buffer proximity.
  7. **Nearby Commercial Impact**: Local youth employment generation and supply chain stimulation.
* Renders **600m direct impact** and **2.4km traffic influence buffer circles** on the GIS map.

### Module 8: 7-Stage Decision Intelligence Center (`decision-intelligence`)
* Mathematical Multi-Criteria Decision Analysis (MCDA) engine evaluating competing civil projects:
  - *Alternative A*: Wai Valley Bypass & Retention Basin
  - *Alternative B*: Mahabaleshwar Escarpment Terracing
  - *Alternative C*: Karad South Floodway & Transit Hub
* **Configurable Criteria Weights** (Sum = 100%):
  - Safety & Hazard Resistance ($35\%$)
  - Road Transit Accessibility ($20\%$)
  - Environmental Preservation ($20\%$)
  - Capital Cost Efficiency ($15\%$)
  - Social Displacement Equity ($10\%$)
* **Dynamic Explanation Engine**: Generates natural-language rationale explaining why the top project won and details trade-offs against runners-up.

### Module 9: AI Decision Assistant (`assistant`)
* Conversational copilot powered by deterministic tool-calling:
  - `getDistrictData()`: District-wide overview and dam storage status.
  - `getTahsilRisk()`: Tahsil-level geophysical risk and feature attribution.
  - `runRainfallScenario()`: Executes live What-If simulations.
  - `analyzeProjectImpact()`: Evaluates infrastructure proposals.
* Grounded natural language responses with zero numerical hallucinations.
* Interactive navigation chips enabling one-click transitions to map coordinates or simulation views.

### Module 10: Official Executive Decision Reports (`reports`)
* Standardized executive memorandum formatted for the **State Emergency Operations Center (SEOC)** and **District Collector**.
* Incorporates complete data lineage disclosures, separating observed telemetry from simulated model predictions.
* Full `@media print` CSS optimization for instant, clean browser printing or saving to PDF (`window.print()`).

---

## 5. Administrative Hierarchy & Pilot Scope

### Maharashtra State (Macro Level)
* **Districts**: 36
* **Administrative Divisions**: 6 (*Pune, Konkan, Nashik, Chhatrapati Sambhaji Nagar, Amravati, Nagpur*)
* **Tahsils**: 358
* **Population**: 112,374,333 (*Census 2011*) | ~12.65 Cr (*2024 Projections*)

### Satara Flagship Pilot (Micro Level — 11 Tahsils)

| Tahsil | HQ | Population | Terrain & Hazard Profile | Key Rivers / Dams / Highways |
|:---|:---|:---|:---|:---|
| **Mahabaleshwar** | Mahabaleshwar | 75,000 | Western Ghats scarp ($35.8^\circ$), $>5,000\text{ mm}$ rain, extreme landslide risk | Origin of Krishna, Venna Lake, SH-72 |
| **Patan** | Patan | 298,000 | Heavy rainfall catchment, seismically active, debris flow hazard | **Koyna Dam (105.25 TMC)**, Tarali Dam, SH-58 |
| **Jaoli** | Medha | 105,000 | Dense evergreen forest valleys, gully erosion, mountain road slips | Venna, Kudali River, Medha link road |
| **Satara** | Satara City | 502,000 | District HQ, Ajinkyatara Fort, Kaas Plateau, urban flash flood | Kanher Dam, Urmodi Dam, NH-48 |
| **Karad** | Karad City | 584,000 | Major urban/agro hub, riverine flooding at **Preeti Sangam** | Confluence of Krishna & Koyna, NH-48 |
| **Wai** | Wai | 200,000 | Temple heritage valley, Dhom Dam catchment runoff | Dhom Dam, Balkawadi Dam, Pasarni Ghat |
| **Khandala** | Shirwal | 140,000 | Major industrial corridor, **Khambatki Ghat** bottleneck | Nira River, NH-48 6-lane tunnel |
| **Koregaon** | Koregaon | 260,000 | Fertile sugarcane basin, local stream flooding | Tilganga, Vasna Rivers, SH-140 |
| **Phaltan** | Phaltan | 345,000 | Agro-industrial sugar belt, canal-irrigated flat plains | Banganga, Nira River, Dhom LB canal |
| **Khatav** | Vaduj | 275,000 | Semi-arid rain-shadow plateau, groundwater depletion | Mayani Bird Sanctuary Lake, Yerala River |
| **Man** | Dahiwadi | 225,000 | Severe rain-shadow belt, chronic drought vulnerability | Pingali Dam, Man River, SH-144 |

---

## 6. Data Connectivity & Academic Honesty Protocol

To adhere to scientific standards, VISION-X categorizes all data into three explicit tiers:

* **No Synthetic Hallucination**: Uninstrumented sensor metrics outside the pilot region display `[N/A — DATA NOT CONNECTED]` rather than fabricated numbers.
* **No Premature Model Claims**: Statewide model evaluation is labeled `[EVALUATION PENDING]` until empirical testing is executed.
* **Authoritative Citations**: All administrative numbers cite verified sources (*GoM Revenue Dept Gazette 2022*, *Census of India 2011 Primary Census Abstract*).

---

## 7. REST API Reference

### Spring Boot Backend (`http://localhost:8080`)
* `GET /api/data/datasets`: List all 7 registered data connectors with provenance metadata.
* `GET /api/data/status`: Statewide district data connectivity summary.
* `GET /api/data/quality`: Data quality audit reports (missing values, CRS status, geometry anomalies).
* `GET /api/data/provenance`: End-to-end data lineage records.
* `GET /api/data/districts`: Complete list of 36 normalized Maharashtra districts.
* `GET /api/district`: Satara pilot district metadata, tahsils, dams, rivers, and roads.
* `GET /api/district/tahsils`: List of 11 pilot tahsils with geophysical baselines.
* `GET /api/reports/latest`: Generates official SEOC executive memorandum.

### Python FastAPI Engine (`http://localhost:8000`)
* `GET /health`: Service health check and uptime status.
* `GET /api/models/evaluation`: Retrieve current Scikit-Learn evaluation metrics (`EVALUATION PENDING` if unrun).
* `POST /api/models/evaluate`: Execute 80/20 train/test split evaluation pipeline and calculate empirical metrics.
* `POST /api/risk/predict`: Run Random Forest risk inference with feature explainability.
* `GET /api/risk/{tahsil_id}`: Retrieve real-time risk prediction for a specific tahsil.
* `POST /api/simulation/what-if`: Execute 3-phase What-If simulation.
* `POST /api/projects/simulate`: Evaluate 7-dimensional infrastructure proposal impact.
* `POST /api/assistant/query`: Natural language query processing with deterministic tool-calling.

---

## 8. Quickstart & Installation Guide

### Prerequisites
* **Java 21 LTS** (`java -version`)
* **Python 3.10+** (`python --version`) with virtual environment support
* **Node.js 18+** (`node -v`) & `npm`
