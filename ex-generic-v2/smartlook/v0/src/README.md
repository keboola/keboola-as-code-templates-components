Extract session data from Smartlook analytics platform to analyze user behavior and improve your website or application experience.

## Configuration
- API Token authentication
- Daily incremental updates
- Automatic pagination handling
- Configurable session filters

### Required Parameters
- `api_token` - Your Smartlook API token for authentication

## Output Data
The template extracts session data into a single table with the following structure:

- `session_id` - Unique identifier of the session (Primary Key)
- `dashboardURL` - Direct link to session recording in Smartlook dashboard
- `pageUrl` - URL of the page where session occurred
- `properties` - Additional session properties and metadata
- `duration` - Length of the session
- `startedAt` - Session start timestamp
- `endedAt` - Session end timestamp

## Features
- Incremental loading of new sessions
- Detailed session information including URLs and properties
- Automatic retry mechanism for API rate limits
- Support for filtering sessions by date range
- Enriched session data with dashboard links

## Links
- [Smartlook API Documentation](https://developers.smartlook.com/reference/api-reference)
- [Generic Extractor Documentation](https://developers.keboola.com/extend/generic-extractor/)
