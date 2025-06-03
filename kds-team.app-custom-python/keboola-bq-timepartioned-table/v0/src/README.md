# BigQuery Time Partitioned Table Creator
To use the component, load the template and fill in the required details. This template will create a typed BigQuery table in storage, with two columns and 0 rows.
1. Primary Key column (can be any type, but must be a unique value). [Bigquery Data types](https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types).
2. Partitioning column. As the table will be partitioned by time, this column must be a DATE or TIMESTAMP

Once you have created your table, you can then use a Keboola BigQuery SQL transformation to add additional columns and rows. 

Create and manage time-partitioned tables in BigQuery directly from Keboola. This template simplifies the process of setting up time-based partitioning for efficient data management and query performance.

## Configuration
- Keboola Stack URL
- Storage API Token
- Bucket ID for table creation
- Table name and structure details
- Partitioning configuration

### Required Parameters
- `keboola_url` - Your Keboola stack URL (e.g., connection.europe-west3.gcp.keboola.com)
- `storage_api_token` - Valid Keboola Storage API token with write access
- `bucket_id` - Target bucket identifier where the table will be created
- `table_name` - Name of the table to be created
- `pk_column_name` - Primary key column name (must be unique, non-null)
- `pk_column_type` - Data type for primary key column
- `partition_column_name` - Column name for time partitioning
- `partition_column_type` - Data type for partition column (DATE or TIMESTAMP)
- `partitioning_type` - Time partitioning granularity (HOUR, DAY, MONTH, or YEAR)

## Output Data
Creates a BigQuery table with:
- Primary key column (specified type, non-nullable)
- Time partition column (DATE or TIMESTAMP)
- Empty initial state (0 rows)
- Time-based partitioning enabled

## Features
- Creates BigQuery-optimized table structure
- Supports multiple time partitioning granularities
- Ensures data integrity with non-null primary key
- Compatible with subsequent transformations
- Allows for future column additions

## Links
- [BigQuery Data Types Documentation](https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types)
- [BigQuery Partitioning Documentation](https://cloud.google.com/bigquery/docs/partitioned-tables)


