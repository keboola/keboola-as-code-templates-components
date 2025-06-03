An AI-powered SQL assistant that helps you interact with your Snowflake database using natural language. This Data App translates your conversational queries into SQL and executes them directly against your database.

## Configuration
- OpenAI API Key for AI capabilities
- Snowflake database connection details
- Account location settings
- Database access credentials

### Required Parameters
- `account_identifier` - Your project location (e.g., keboola.west-europe.azure)
- `openai_api_key` - Your OpenAI API key for AI functionality
- `warehouse_name` - Snowflake warehouse name (e.g., KEBOOLA_PROD)
- `database_name` - Your Snowflake database name
- `schema_name` - Database schema to query
- `user` - Database user/account name
- `password` - Database access password

## Output Data
- Dynamic SQL query results based on your natural language questions
- Query history for reference
- Explanation of generated SQL queries

## Features
- Natural language to SQL translation
- Interactive chat interface
- Real-time query execution
- Query explanation and documentation
- Support for complex database operations
- History tracking of conversations and queries

## Links
- [Snowflake Documentation](https://docs.snowflake.com/)
- [OpenAI API Documentation](https://platform.openai.com/docs/introduction)
- [Keboola Documentation](https://help.keboola.com/)
