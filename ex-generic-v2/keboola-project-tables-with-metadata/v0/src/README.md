Extract detailed information about tables and their metadata from your Keboola project to monitor and analyze your data structures.

## Configuration
- Extracts table information from Keboola Storage API including metadata, buckets, columns, and column metadata
- Comprehensive data mapping for all table attributes and related information
- Non-incremental loading to ensure complete table information
- Detailed error handling and response processing

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage API token with access to table information
- `kbc_hostname` - Your Keboola project hostname (e.g., connection.north-europe.azure.keboola.com)

## Output Data
The template creates two output tables:

`tables` - Contains table information with columns:
- `table_id` (Primary Key)
- `table_name` - Name of the table
- `bucket_id` - ID of the bucket containing the table
- `rows_count` - Number of rows in the table
- `data_size_bytes` - Size of the table data
- `created`, `last_change_date`, `last_import_date` - Timestamps
- `is_alias`, `is_typed`, `transactional` - Table properties
- `primary_keys`, `distribution_keys`, `index_keys` - Key configurations
- Additional metadata fields and configuration details

`table_bucket` - Contains bucket information with columns:
- `bucket_id` (Primary Key)
- `table_id` (Primary Key) - Reference to parent table
- `bucket_name` - Name of the bucket
- `stage` - Bucket stage (in/out)
- `sharing` - Sharing configuration
- `created`, `last_change_date` - Timestamps
- Additional bucket properties and metadata

## Features
- Complete table structure analysis
- Bucket and metadata tracking
- Column-level information extraction
- Detailed sharing and permission tracking
- Comprehensive table properties monitoring

## Links
- [Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
- [Storage API Documentation](https://help.keboola.com/api/storage/)
- [Table Management Guide](https://help.keboola.com/storage/tables/)
