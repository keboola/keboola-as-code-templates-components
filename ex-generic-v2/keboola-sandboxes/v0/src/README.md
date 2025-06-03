Extract information about Keboola sandboxes in your project using the Generic Extractor component.

## Configuration
- Uses Generic Extractor v2 to fetch sandbox data
- Connects to Keboola Sandboxes API
- Extracts sandbox details and metadata

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage Token or Master Token for API authentication
- `kbc_hostname` - Your project's Keboola hostname (e.g., "north-europe.azure.keboola.com")

## Output Data
- `sandboxes` - List of all sandboxes in your project including:
  - Sandbox ID and name
  - Creation and expiration dates
  - Size and type
  - Status information
  - Associated user details

## Features
- Incremental updates supported
- Detailed sandbox metadata extraction
- Automatic API authentication
- Debug mode available

## Links
- [Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
- [Keboola Sandboxes API Documentation](https://api.keboola.com/)
