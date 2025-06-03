Extract and analyze Google Ads ad groups and campaign performance data to optimize your advertising strategy.

## Configuration
- OAuth authentication with Google Ads
- Date range selection for data extraction
- Automated data extraction from Google Ads API

### Required Parameters
- `oauth-googleads` - Google Ads authorization credentials
- `oauth-googleads-accounts` - Selected Google Ads accounts
- `ex-google-ads-since` - Start date for data extraction (default: last week)
- `ex-google-ads-until` - End date for data extraction (default: now)

## Output Data

### Ad Groups Table
- Date segmentation
- Ad group ID and name
- Status and type
- Campaign association
- Performance metrics:
  - Clicks
  - Conversions
  - Engagement rate
  - Cost per conversion
  - Cost (in micros)
  - CTR

### Campaigns Table
- Date segmentation
- Campaign ID and name
- Status and channel type
- Start/end dates
- Performance metrics:
  - Clicks
  - Impressions
  - Cost per conversion
  - Engagement rate

## Features
- Daily performance metrics for ad groups
- Campaign-level analytics
- Cost and conversion tracking
- Engagement and CTR analysis
- Historical data analysis

## Links
- [Google Ads API Documentation](https://developers.google.com/google-ads/api/docs/start)
- [Keboola Google Ads Extractor Documentation](https://help.keboola.com/components/extractors/marketing-sales/google-ads/)
