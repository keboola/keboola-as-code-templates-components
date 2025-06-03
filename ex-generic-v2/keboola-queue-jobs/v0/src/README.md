Extract detailed information about jobs and their execution from your Keboola Queue API to monitor and analyze workload performance.

## Configuration
- Extracts job information from Keboola Queue API including execution details, metrics, and results
- Incremental loading to track job history efficiently
- Comprehensive data mapping for all job attributes and related information
- Detailed error handling and response processing

### Required Parameters
- `kbc_storage_token` - Your Keboola Storage API token with access to job information
- `kbc_hostname` - Your Keboola project hostname (e.g., connection.north-europe.azure.keboola.com)

## Output Data
The template creates one output table:

`jobs_union` - Contains job information with columns:
- `run_id` (Primary Key) - Unique identifier for each job run
- `job_id` - ID of the job
- `project_id`, `project_name` - Project information
- `component` - Component that executed the job
- `config` - Configuration ID
- `status`, `desired_status` - Job status information
- `start_time`, `end_time`, `created_time` - Execution timestamps
- `duration_seconds` - Job duration
- Various metrics columns (storage, backend metrics)
- Input/output tables information
- Token and execution context details
- Additional metadata and configuration fields

## Features
- Complete job execution tracking
- Performance metrics collection
- Resource usage monitoring
- Error tracking and analysis
- Comprehensive execution context capture

## Links
- [Queue API Documentation](https://developers.keboola.com/integrate/jobs/)
- [Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
- [Job Management Guide](https://help.keboola.com/management/jobs/)
