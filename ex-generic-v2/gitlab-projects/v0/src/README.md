This template helps you extract data from GitLab projects including project details and merge requests using the GitLab API v4.

## Configuration
- Uses GitLab API v4 endpoint
- Extracts both project and merge request data
- Supports pagination with 100 items per page
- Handles private project visibility
- Includes incremental updates for merge requests

### Required Parameters
- `api_token` - GitLab API token with read access to projects
- `project_id` - ID of the GitLab project to extract data from

## Output Data

### Projects Table
Contains basic project information:
- Project ID
- Name
- Description
- Visibility
- Created/Updated timestamps
- Repository details
- Other project metadata

### Merge Requests Table
Contains merge request data:
- MR ID
- Title
- State
- Source/Target branches
- Author information
- Created/Updated timestamps
- Associated project ID

## Features
- Extracts complete project metadata
- Retrieves all merge requests for the project
- Supports incremental loading of merge requests
- Handles API pagination automatically
- Ignores 404 errors gracefully

## Links
- [GitLab API Documentation](https://docs.gitlab.com/ee/api/projects.html)
- [GitLab Merge Requests API](https://docs.gitlab.com/ee/api/merge_requests.html)
- [Keboola Generic Extractor Documentation](https://help.keboola.com/components/extractors/other/generic/)
