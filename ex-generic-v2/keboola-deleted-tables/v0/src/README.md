Extract and monitor deleted table events from your Keboola project to track table deletions over time.

## Configuration
- Extracts events from Keboola Storage API filtered for table deletion events
- Incremental loading enabled by default
- Pagination set to 100 records per request with a 10,000 record limit
- Events are filtered using query "event:storage.tableDeleted"

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage API token with access to events
- `kbc_hostname` - Your Keboola project hostname (e.g., connection.north-europe.azure.keboola.com)
- `kbc_project_id` - ID of the project to monitor for deleted tables

## Output Data
The template creates one output table:

`events` - Contains table deletion event records with the following columns:
- `id`, `runId`, `projectId` (Primary Keys)
- `event` - Type of event (storage.tableDeleted)
- `created` - Event timestamp
- `message` - Event description
- `type` - Event classification
- `objectId` - ID of the deleted table
- `objectName` - Name of the deleted table
- `objectType` - Type of the deleted object
- Additional metadata fields (token info, parameters, etc.)

## Features
- Incremental updates to avoid duplicate data
- Detailed tracking of table deletions
- Automatic error handling and retry logic
- Configurable pagination settings
- Primary key enforcement for data consistency

## Links
- [Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
- [Keboola Events API Documentation](https://keboola.docs.apiary.io/#reference/events)
- [Storage API Documentation](https://help.keboola.com/api/storage/)
