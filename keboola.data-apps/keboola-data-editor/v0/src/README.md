A powerful data editing interface that allows business users to directly view and modify data stored in Keboola Storage tables through an intuitive spreadsheet-like interface, eliminating the need for data exports and external tools.

## Configuration
- Storage token configuration with specific bucket/folder access rights
- Field/column editing limitations and validations
- User access controls and permissions
- Table selection and editing capabilities

### Required Parameters
- `kbc_storage_token` - Keboola Storage token with appropriate read/write permissions for target tables

## Output Data
- Modified tables in Keboola Storage
- Changes applied through full load or incremental updates (when primary keys are set)
- Audit trail of modifications

## Features
- Direct table editing in spreadsheet format
- Real-time data validation
- Immediate changes reflection in Keboola Storage
- Support for both full and incremental updates
- User-friendly interface for non-technical users
- Column-level access control
- Built-in data validation rules
- Change history tracking

## Links
- [Interactive Keboola Sheets Documentation](https://help.keboola.com/templates/interactive-keboola-sheets/)
- [Keboola Storage API Documentation](https://developers.keboola.com/integrate/storage/)
- [Data Apps Documentation](https://help.keboola.com/components/applications/)