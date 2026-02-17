# retail-data-lakehouse-pipeline
retail-data-lakehouse-pipeline-folder/
│
├── data/
│   ├── parent_company/
│   │   ├── full_load/
│   │   │   ├── dim_customers.csv
│   │   │   ├── dim_gross_price.csv
│   │   │   ├── dim_products.csv
│   │   │   └── fact_orders.csv
│   │   │
│   │   └── incremental_load/
│   │       ├── fact_orders.csv
│   │       └── incremental_data_parent-company_query.txt
│   │
│   └── child_company/
│       ├── full_load/
│       │   ├── customers/
│       │   │   └── customers.csv
│       │   │
│       │   ├── gross_price/
│       │   │   └── gross_price.csv
│       │   │
│       │   ├── orders/
│       │   │   └── landing/
│       │   │       └── 151 CSV files
│       │   │
│       │   └── products/
│       │       └── products.csv
│       │
│       └── incremental_load/
│           └── orders/
│               └── 31 CSV files
│
├── codes/
│   ├── setup/
│   │   └── dim_date_table_creation.ipynb
│   │   └── setup_catalog.ipynb
│   │   └── utilities.ipynb
│   │
│   ├── dimension_data_processing/
│   │   └── customers_data_processing.ipynb
│   │   └── products_data_processing.ipynb
│   │   └── pricing_data_processing.ipynb
│   │
│   └── fact_data_processing/
│   │   └── full_load_fact.ipynb
│   │   └── incremental_load_fact.ipynb
│
├── dashboarding/
│   ├── denormalize_table_query.txt
│   └── dashboard_report.pdf
│
└── resources/
    ├── databricks_project.excalidraw
    └── project_architecture.png
