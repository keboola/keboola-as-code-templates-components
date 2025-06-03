# Google Analytics Traffic Acquisition Template

This template helps you analyze website traffic sources and user behavior by extracting key acquisition metrics from Google Analytics 4.

## Configuration
- Google Analytics account authorization
- Date range selection for data extraction
- Automatic data refresh settings

### Required Parameters
- `oauth-google-analytics` - Google Analytics authorization
- `oauth-google-analytics-accounts` - Selected GA4 properties
- `ga-from` - Start date for data collection (1 week to 2 months ago)
- `ga-to` - End date for data collection (1 day to 1 week ago)

## Output Data
- `traffic_acquisition` - Contains daily traffic metrics:
  - Source, medium, and campaign data
  - New vs returning visitors
  - Active users and session metrics
  - Engagement metrics
  - User behavior statistics

## Features
- Daily traffic source analysis
- Campaign performance tracking
- User engagement metrics
- Session quality measurements
- New vs returning visitor segmentation
- Automated data extraction

## Links
- [Google Analytics 4 Documentation](https://developers.google.com/analytics/devguides/reporting/data/v1)
- [GA4 Dimensions & Metrics Reference](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema)

