Monitor and analyze your Keboola Storage usage by extracting detailed information about all tables in your project.

## Configuration
- Extracts table metadata using Keboola Storage API
- Runs incrementally to track changes over time
- Includes comprehensive table statistics and metrics

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage or master token for API access
- `kbc_hostname` - Your project's hostname (e.g., connection.north-europe.azure.keboola.com)

## Output Data
The template creates a single output table containing:
- `dataSizeBytes` - Size of the table in bytes
- `rowsCount` - Number of rows in the table
- `created` - Table creation timestamp
- `lastChangeDate` - Last modification timestamp
- `lastImportDate` - Last data import timestamp
- `name` - Table name
- `id` - Table ID
- `bucket_backend` - Storage backend type
- `uri` - Table URI

## Features
- Automated table size monitoring
- Historical storage usage tracking
- Table metadata collection
- Incremental updates
- Support for all Keboola regions

## Links
- [Keboola Storage API Documentation](https://developers.keboola.com/integrate/storage/)
- [Generic Extractor Documentation](https://developers.keboola.com/extend/generic-extractor/)
