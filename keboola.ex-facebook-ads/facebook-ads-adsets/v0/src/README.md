# Facebook Ads Ad Sets

This template extracts data about your Facebook Ads ad sets and their performance metrics. It provides insights into how different audience segments and targeting strategies are performing across your campaigns.

## Configuration
- Extracts ad sets data and insights from the Facebook Ads API
- Collects last month's performance metrics with daily granularity
- Includes campaign structure for proper data hierarchy
- Automatically handles API pagination

### Required Parameters
- `oauth-facebookads` - Facebook Ads authorization credentials
- `oauth-facebookads-accounts` - Selected Facebook Ad accounts to extract data from

## Output Data
The template creates following tables:
- `campaigns` - Basic campaign information (ID, name, status)
- `adsets` - Ad set details and their relationship to campaigns
- `adsets_insights` - Daily performance metrics for each ad set including:
  - Impressions
  - Reach
  - Clicks
  - Spend
  - Actions/Conversions

## Features
- Automated daily performance metrics collection
- Campaign hierarchy mapping
- Ad set level targeting insights
- Spend and performance tracking
- Multi-account support

## Links
- [Facebook Ads API Documentation](https://developers.facebook.com/docs/marketing-api/reference)
- [Facebook Ads Components in Keboola](https://help.keboola.com/components/extractors/marketing-sales/facebook-ads/)
