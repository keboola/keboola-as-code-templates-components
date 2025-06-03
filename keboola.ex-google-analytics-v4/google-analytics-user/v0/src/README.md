# Google Analytics User Acquisition Template

Extract detailed user acquisition and demographic data from your Google Analytics 4 property to analyze user behavior and engagement patterns.

## Configuration
- Google Analytics 4 account connection
- Configurable date range for data extraction
- Automatic data refresh settings

### Required Parameters
- `oauth-google-analytics` - Google Analytics authorization
- `oauth-google-analytics-accounts` - Selected GA4 property
- `ga-from` - Start date for data extraction (default: 1 month ago)
- `ga-to` - End date for data extraction (default: 1 day ago)

## Output Data
- `user_acquisition` table containing:
  - User metrics (total, active, new users)
  - Engagement metrics (sessions, duration, event counts)
  - Demographic data (age, gender, country)
  - New vs returning user breakdown
  - Daily granularity

## Features
- Complete user behavior analysis
- Demographic segmentation
- Engagement metrics tracking
- New vs returning user comparison
- Daily trend analysis
- Automated data updates

## Links
- [Google Analytics 4 API Documentation](https://developers.google.com/analytics/devguides/reporting/data/v1)
- [GA4 Dimensions & Metrics Reference](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema)

