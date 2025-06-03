Extract and monitor events from specific Keboola configurations to track changes, runs, and activities over time.

## Configuration
- Extracts events from Keboola Storage API for a specific component configuration
- Incremental loading enabled by default
- Pagination set to 100 records per request with a 10,000 record limit
- Events are filtered by component ID and configuration ID

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage API token with access to events
- `kbc_hostname` - Your Keboola project hostname (e.g., connection.north-europe.azure.keboola.com)
- `kbc_component_id` - ID of the component to monitor (e.g., keboola.snowflake-transformation)
- `kbc_configuration_id` - ID of the specific configuration to track

## Output Data
The template creates one output table:

`events` - Contains configuration event records with the following columns:
- `id`, `runId` (Primary Keys)
- `event` - Type of event that occurred
- `component` - Component identifier
- `configurationId` - Configuration being monitored
- `created` - Event timestamp
- `message` - Event description
- `type` - Event classification
- Additional context fields (token, user agent, API version, etc.)

## Features
- Incremental updates to avoid duplicate data
- Detailed event tracking with full context
- Automatic error handling and retry logic
- Configurable pagination settings
- Primary key enforcement for data consistency

## Links
- [Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
- [Keboola Events API Documentation](https://keboola.docs.apiary.io/#reference/events)
- [Storage API Documentation](https://help.keboola.com/api/storage/)
