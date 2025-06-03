This template extracts detailed pipeline data from your GitLab projects. It provides comprehensive insights into your CI/CD processes by collecting information about pipelines, jobs, and pipeline bridges.

## Configuration
- Extracts data from private GitLab projects
- Uses GitLab API v4
- Collects data from the last 3 days
- Includes retried jobs
- Handles pagination (100 items per page)

### Required Parameters
- `api_token` - GitLab API token with access to your repositories

## Output Data

### Projects Table
- Project ID and visibility settings
- Project metadata

### Pipelines Table
- `pipeline_id` - Unique pipeline identifier
- `project_id` - Associated project ID
- `status` - Current pipeline status
- `ref` - Git reference (branch/tag)
- `created_at`, `updated_at`, `started_at`, `finished_at` - Timing information
- `duration` - Pipeline execution time
- `coverage` - Code coverage data
- `user_name`, `user_username` - Pipeline trigger user
- Detailed status information (icon, text, label, group)

### Jobs Table
- `id` - Job identifier
- `pipeline_id` - Associated pipeline
- `stage` - Pipeline stage
- `status` - Job status
- `duration` - Execution time
- `created_at`, `started_at`, `finished_at` - Timing information
- `user_name`, `user_username` - Job executor
- `web_url` - Direct link to job

### Bridges Table
- `bridge_id` - Bridge identifier
- `parent_pipeline_id` - Source pipeline
- `child_pipeline_id` - Target pipeline
- `status` - Bridge status
- `name` - Bridge name
- `user_name`, `user_username` - Associated user

## Features
- Incremental updates supported
- Error handling for 404 responses
- Detailed pipeline execution tracking
- Cross-project pipeline relationships via bridges
- Complete job history including retries

## Links
- [GitLab API Documentation](https://docs.gitlab.com/ee/api/pipelines.html)
- [GitLab CI/CD Documentation](https://docs.gitlab.com/ee/ci/)
