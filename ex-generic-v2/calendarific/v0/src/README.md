This template uses the Generic Extractor to retrieve national holiday data from the Calendarific API, helping you maintain an up-to-date calendar of holidays for multiple countries.

## Configuration

The template is configured to:
- Fetch only national holidays (type='national')
- Use incremental loading for efficient updates
- Support multiple countries in parallel:
  - Czech Republic (CZ)
  - Canada (CA) 
  - United States (US)
  - Great Britain (GB)

### Required Parameters

- `api_token` - Your Calendarific API key from your account dashboard
- `year` - Target year for holiday data (e.g., "2024")

## Output Tables

The template creates separate tables for each country's holidays:
- `holidays_cz` - Czech national holidays
- `holidays_ca` - Canadian national holidays  
- `holidays_us` - US national holidays
- `holidays_gb` - British national holidays

Each table contains:
- `date` - Holiday date in ISO format (e.g., "2024-12-25"), serves as primary key
- `name` - Official holiday name (e.g., "Christmas Day")

## Features

- Incremental loading to prevent duplicate data
- Data retrieved via Calendarific API v2
- National holiday filtering
- Primary key constraints for data integrity
- Multi-country support in single configuration

## Links

- [Calendarific API Documentation](https://calendarific.com/api-documentation)
- [Generic Extractor Documentation](https://developers.keboola.com/extend/generic-extractor/)
