# Google Analytics Events Engagement Template

Extract detailed event engagement metrics from your Google Analytics 4 property to analyze user interactions and event performance.

## Configuration
- Google Analytics 4 account connection
- Customizable date range for data extraction
- Event engagement metrics selection

### Required Parameters
- `oauth-google-analytics` - Google Analytics authorization
- `oauth-google-analytics-accounts` - Selected GA4 property
- `ga-from` - Start date for data extraction (default: 1 month ago)
- `ga-to` - End date for data extraction (default: 1 day ago)

## Output Data
- `events_engagement` table containing:
  - Event name and date
  - Event counts and counts per user
  - Active and total users
  - Event value and total revenue
  - Key event status

## Features
- Daily event engagement metrics
- Revenue tracking per event
- Key events identification
- User engagement analysis
- Flexible date range selection

## Links
- [Google Analytics 4 Documentation](https://developers.google.com/analytics/devguides/reporting/data/v1)
- [GA4 Events Reference](https://support.google.com/analytics/answer/9322688)

