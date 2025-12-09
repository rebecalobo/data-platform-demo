# data-platform-demo

Fluxo principal:

- Extract — coleta via API (requests) + ingestão de arquivos (CSV/JSON/Excel)
- Raw — salva brutos em Parquet
- Process (PySpark) — limpeza, transformação, enriquecimento e agregações em larga escala
- DW — materializa dimensões e fatos (Parquet / DuckDB / Postgres)
- Orquestração — Airflow controlando Extract → Spark Jobs → Load → Quality
