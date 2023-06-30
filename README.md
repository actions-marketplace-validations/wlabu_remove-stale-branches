# Remove stale branches
Github Action to notify people when branches are stale, and delete the branch if no action is taken.

> This action searches Slack for the branch author's email address (i.e.: their Git user email), and notifies them if found.

## Requirements

Along with installing the action in your project's `.github` directory, you will need to create 2 environment variables:
- `GH_TOKEN_FOR_STALE_BRANCHES`: An access token with `repo` permissions
- `SLACK_TOKEN_FOR_STALE_BRANCHES`: An access token with the following "Bot Token Scopes":
    - chat:write
    - users:read
    - users:read.email

> This means you will most probably need to create a Slack app, if you don't have a token already.
