# Google Analytics Landing Page Engagement

Extract detailed landing page performance metrics from Google Analytics 4 to analyze how visitors engage with your website entry points.

## Configuration
- Google Analytics 4 account connection
- Customizable date range for data extraction
- Automatic data refresh options

### Required Parameters
- `oauth-google-analytics` - Google Analytics authorization
- `oauth-google-analytics-accounts` - Selected GA4 properties to extract data from
- `ga-from` - Start date for data extraction (1 week to 2 months ago)
- `ga-to` - End date for data extraction (1 day to 1 week ago)

## Output Data
The template creates one table:
- `landing_page_engagement` - Contains metrics per landing page:
  - Landing page URL and query parameters
  - Device category
  - Active, new and total users
  - Sessions and engaged sessions
  - Page views
  - Average session duration
  - User engagement duration
  - Event count

## Features
- Extracts comprehensive landing page performance metrics
- Segments data by device category
- Tracks both basic and advanced engagement metrics
- Supports multiple GA4 properties
- Customizable date ranges for analysis

## Links
- [Google Analytics 4 Documentation](https://developers.google.com/analytics/devguides/reporting/data/v1)
- [GA4 Dimensions & Metrics Reference](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema)

