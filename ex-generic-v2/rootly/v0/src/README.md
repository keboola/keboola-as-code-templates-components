Extract incident and team data from your Rootly instance to analyze incident management performance and team structures.

## Configuration
- API Token authentication
- Automatic pagination handling
- Error handling for 404 responses
- Data extraction for incidents and teams

### Required Parameters
- `api_token` - Your Rootly API token for authentication

## Output Data

### Incidents Table
- `id` - Unique incident identifier (Primary Key)
- `title` - Incident title
- `slug` - URL-friendly identifier
- `status` - Current incident status
- `started_at` - Incident start timestamp
- `mitigated_at` - Mitigation timestamp
- `resolved_at` - Resolution timestamp
- `started_by_user_email` - Email of user who reported incident
- `team_id` - Associated team identifier
- `severity` - Incident severity level
- `jira_issue_id` - Associated Jira ticket ID

### Teams Table
- `id` - Unique team identifier (Primary Key)
- `name` - Team name
- `description` - Team description

## Features
- Real-time incident data extraction
- Team structure and organization mapping
- Incident lifecycle tracking
- Integration with Jira tickets
- Severity level monitoring
- Incident ownership tracking

## Links
- [Rootly API Documentation](https://docs.rootly.com/reference/getting-started-with-rootly-api)
- [Rootly Homepage](https://rootly.com)
