# Sample Code Structure for VPDIP

Recommended repository structure:

```
vital-parks-data-platform/
├── src/
│   ├── data_ingestion/          # Pipeline scripts for sensors, mobility APIs, etc.
│   ├── data_processing/         # Cleaning, feature engineering, ETL
│   ├── models/                  # Analytical models (visitation, accessibility)
│   ├── visualization/           # Tableau prep, dashboards, plots
│   └── utils/                   # Reusable modules
├── notebooks/                   # Exploratory analysis (Jupyter)
├── pipelines/                   # Airflow DAGs or dbt models
├── docker/                      # Container configs
├── docs/                        # Documentation
├── tests/                       # Unit and integration tests
├── .github/workflows/           # CI/CD
├── data/                        # Sample or schema files (gitignored raw data)
└── requirements.txt / environment.yml
```

**Example files to create:**
- `src/data_ingestion/sensor_ingest.py`
- `src/models/visitation_model.py`
- `pipelines/daily_update_dag.py`
