# ADF_PRO

1. Ingestion Pipeline

This pipeline performs incremental data ingestion from source files into Azure SQL Database using a timestamp-based watermark approach. It checks for new records, conditionally loads updated data, and updates the last processed timestamp for efficient ETL execution.

2. RestAPI Pipeline

This pipeline extracts data from external REST API endpoints and ingests the response into Azure storage for further processing. It enables automated API-based data integration and supports dynamic dataset handling.

3. Router Pipeline

This pipeline acts as a control workflow that routes data processing based on conditions such as file type, record availability, or ingestion status. It ensures modular execution by triggering the appropriate pipeline path.

4. Scheduled Pipeline

This pipeline is designed for time-based automation and orchestration of ETL jobs. It triggers ingestion workflows on a defined schedule to ensure continuous and up-to-date data movement.
