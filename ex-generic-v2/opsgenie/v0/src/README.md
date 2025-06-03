Extract key operational data from your Opsgenie instance including alerts, teams, users, and on-call schedules.

## Configuration
- Incremental updates for alerts data
- 3-day lookback window for alert updates
- 12-month timeline for schedules
- Pagination set to 100 records per request

### Required Parameters
- `api_token` - Your Opsgenie API token with read access to alerts, teams, users, and schedules

## Output Data

### Teams (`ex-opsgenie.teams`)
- Team ID, name, description
- API and web interface links

### Users (`ex-opsgenie.users`) 
- User ID, username, full name
- Role information and timezone
- Account status (blocked/verified)
- Creation timestamp

### Alerts (`ex-opsgenie.alerts`)
- Alert ID and details (message, priority, status)
- Creation and update timestamps
- Integration details
- Team and owner information
- Alert lifecycle data (acknowledged, seen, snoozed)

### Schedules (`ex-opsgenie.schedules`)
- Schedule configurations
- Timeline data for on-call rotations
- Coverage information

## Features
- Incremental loading of alert data
- Complete team and user roster extraction
- Detailed alert history with status tracking
- On-call schedule timeline extraction
- Automatic data type mapping
- Error handling and retry logic

## Links
- [Opsgenie API Documentation](https://docs.opsgenie.com/docs/api-overview)
- [Generic Extractor Documentation](https://developers.keboola.com/extend/generic-extractor/)
