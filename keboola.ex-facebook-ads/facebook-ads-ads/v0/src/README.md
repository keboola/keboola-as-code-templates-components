Extract detailed Facebook Ads data including campaigns, ad sets, ads, and their performance insights.

## Configuration
- Facebook Ads account authorization via OAuth
- Automatic extraction of all accessible ad accounts
- Configurable data retrieval period (default: last month)
- Rate limits and pagination handled automatically

### Required Parameters
- `oauth-facebookads` - Facebook Ads authentication credentials
- `oauth-facebookads-accounts` - Selection of Facebook Ad accounts to extract data from

## Output Data
- `campaigns` - Campaign level data including ID, name, account ID, and status
- `adsets` - Ad set information with ID, name, and campaign association
- `ads` - Individual ad data with ID, name, and ad set relationship
- `ads_insights` - Daily performance metrics including:
  - Impressions
  - Reach
  - Actions
  - Clicks
  - Spend

## Features
- Incremental updates supported
- Daily granularity for performance metrics
- Automatic handling of API pagination
- Nested data structure extraction
- Error handling and retry mechanisms

## Links
- [Facebook Marketing API Documentation](https://developers.facebook.com/docs/marketing-apis/)
- [Keboola Facebook Ads Extractor Documentation](https://help.keboola.com/components/extractors/marketing-sales/facebook-ads/)
