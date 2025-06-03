Extract detailed Google Ads performance data including campaigns, ad groups, and individual ads metrics.

## Configuration
- OAuth authentication with Google Ads
- Date range selection for data extraction
- Automatic extraction of campaigns, ad groups and ads data
- Customizable data refresh frequency

### Required Parameters
- `oauth-googleads` - Google Ads authentication credentials
- `oauth-googleads-accounts` - Selected Google Ads accounts for data extraction
- `ex-google-ads-since` - Start date for data extraction (default: last week)
- `ex-google-ads-until` - End date for data extraction (default: now)

## Output Data
- `campaigns` - Campaign performance metrics including impressions, clicks, costs and conversions
- `ad_groups` - Ad group level metrics with engagement rates and conversion costs
- `ads` - Individual ad performance data with detailed metrics and status

## Features
- Comprehensive Google Ads data extraction
- Daily granularity of performance metrics
- Multiple account support
- Historical data loading capabilities
- Automated data refresh
- Key performance metrics tracking

## Links
- [Google Ads API Documentation](https://developers.google.com/google-ads/api/docs/start)
- [Keboola Google Ads Extractor Documentation](https://help.keboola.com/components/extractors/marketing-sales/google-ads/)
