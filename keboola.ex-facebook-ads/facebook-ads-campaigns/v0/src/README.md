Extract and analyze your Facebook Ads campaign performance data with this template. Get insights into campaign metrics, spending, and engagement across your Facebook advertising accounts.

## Configuration
- Facebook Ads account authorization via OAuth
- Automatic data extraction for all accessible ad accounts
- Configurable date range for campaign insights (default: last month)
- Daily granularity for performance metrics

### Required Parameters
- `oauth-facebookads` - Facebook Ads authentication credentials
- `oauth-facebookads-accounts` - Selection of Facebook Ad accounts to extract data from

## Output Data
- `campaigns` - Basic campaign information including:
  - Campaign ID and name
  - Account ID
  - Campaign status
- `campaigns_insights` - Daily performance metrics including:
  - Impressions and reach
  - Click data
  - Actions/conversions
  - Campaign spend
  - Campaign ID (for joining with campaigns table)

## Features
- Automated daily campaign performance tracking
- Complete campaign metadata extraction
- Detailed engagement and conversion metrics
- Cost and ROI analysis capabilities
- Multi-account support

## Links
- [Facebook Ads API Documentation](https://developers.facebook.com/docs/marketing-apis/)
- [Keboola Facebook Ads Extractor Documentation](https://help.keboola.com/components/extractors/marketing-sales/facebook-ads/)
