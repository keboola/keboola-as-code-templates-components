Extract and analyze your Google Ads campaign performance data with this template. Get insights into campaign metrics like impressions, clicks, costs, and engagement rates across all your Google Ads accounts.

## Configuration
- Date range selection for data extraction
- OAuth authentication for secure Google Ads access
- Support for multiple Google Ads accounts

### Required Parameters
- `oauth-googleads` - Google Ads authentication credentials
- `oauth-googleads-accounts` - Selected Google Ads accounts for data extraction
- `ex-google-ads-since` - Start date for data extraction (default: last week)
- `ex-google-ads-until` - End date for data extraction (default: now)

## Output Data
The template extracts campaign performance data including:
- Campaign ID and name
- Campaign status and type
- Start and end dates
- Daily performance metrics:
  - Clicks
  - Impressions
  - Cost per conversion
  - Engagement rate

## Features
- Daily campaign performance tracking
- Multiple date range options
- Support for all advertising channel types
- Key performance metrics extraction
- Multi-account data aggregation

## Links
- [Google Ads API Documentation](https://developers.google.com/google-ads/api/docs/start)
- [Keboola Google Ads Extractor Documentation](https://help.keboola.com/components/extractors/marketing-sales/google-ads/)
