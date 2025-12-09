# Data Pipeline Saúde

O objetivo é demonstrar competências práticas em ETL/ELT, extração via API, ingestão de arquivos, tratamento e padronização de dados em larga escala com PySpark, modelagem de Data Warehouse, orquestração com Airflow e empacotamento com Docker.

Fluxo principal:

- Extract — coleta via API (requests) + ingestão de arquivos (CSV/JSON/Excel)
- Raw — salva brutos em Parquet
- Process (PySpark) — limpeza, transformação, enriquecimento e agregações em larga escala
- DW — materializa dimensões e fatos (Parquet / DuckDB / Postgres)
- Orquestração — Airflow controlando Extract → Spark Jobs → Load → Quality
