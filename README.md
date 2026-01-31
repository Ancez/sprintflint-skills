# SprintFlint Agent Skills

Agent skills for interacting with SprintFlint through the REST API.

## Installation

Add this repository to your Cursor skills directory or reference it in your agent configuration.

## Available Skills

- **sprintflint-api** - Comprehensive skill for managing projects, sprints, issues, and comments via the SprintFlint REST API

## Authentication

All API requests require an API token. Get your token from your SprintFlint account settings.

Set the `SPRINTFLINT_API_TOKEN` environment variable or pass the token in the `X-API-Token` header.

## API Base URL

- Production: `https://sprintflint.com/api/v1`

## Usage

Reference the skill in your agent or use the API documentation directly:

```
Use the sprintflint-api skill to create a new issue in the current sprint.
```

## License

MIT
