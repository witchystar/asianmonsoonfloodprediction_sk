# Asian Monsoon Flood Prediction & Risk Index
## High-Resolution Meteorological, Topographical, and Land-Cover Datasets for Advanced Natural Disaster Modeling

### Context
Accurate flood risk assessment across South and Southeast Asia requires accounting for complex interactions between monsoonal climate anomalies, regional topography, and human-driven environmental modifications. This benchmark dataset merges simulated multi-modal features calibrated against historical river basin profiles from 2015 to 2026.

### Data Dictionary Table

| Column Name | Data Type | Measurement Unit | Description & Physical Meaning |
| :--- | :--- | :--- | :--- |
| `Region_ID` | Categorical | Text String | Identifier for specific South/Southeast Asian river basins and deltas. |
| `Monsoon_Intensity_Index` | Continuous | Index (0–100) | Normalized seasonal rainfall anomaly score compared to historical baselines. |
| `Topographic_Wetness_Index` | Continuous | Dimensionless | Quantifies water accumulation tendency based on local slope and catchment area. |
| `River_Discharge_Rate_CMS` | Continuous | Cubic Meters / Sec ($m^3/s$) | Main river channel water volume passing per second during peak flow windows. |
| `Deforestation_Rate_Pct` | Continuous | Percentage (%) | Percentage of forest cover lost within the local watershed over the decade. |
| `Urban_Impervious_Pct` | Continuous | Percentage (%) | Ratio of artificial surfaces preventing natural water infiltration. |
| `Soil_Moisture_Anomaly` | Continuous | Scaled (0–1) | Relative saturation of topsoil layers prior to heavy precipitation events. |
| `Flood_Target_Binary` | Binary | Integer (0 or 1) | Target label: `1` indicates damaging flooding occurred; `0` normal conditions. |

### Provenance & Methodology
Engineered using statistical bounds reflecting ERA5 reanalysis distributions and HydroSHEDS topographical constraints for high-performance machine learning validation.
