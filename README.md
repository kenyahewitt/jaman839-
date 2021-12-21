
# Haikus for Codespaces

    # Only pull requests with all of these labels are checked if stale. Defaults to `[]` (disabled) and can be a comma-separated list of labels. Override "only-labels" option regarding only the pull requests.
    only-pr-labels: # optional, default is 
    # The maximum number of operations per run, used to control rate limiting (GitHub API CRUD related).
    operations-per-run: # optional, default is 30
    # Remove stale labels from issues and pull requests when they are updated or commented on.
    remove-stale-when-updated: # optional, default is true
    # Remove stale labels from issues when they are updated or commented on. Override "remove-stale-when-updated" option regarding only the issues.
    remove-issue-stale-when-updated: # optional, default is 
    # Remove stale labels from pull requests when they are updated or commented on. Override "remove-stale-when-updated" option regarding only the pull requests.
    remove-pr-stale-when-updated: # optional, default is 
    # Run the processor in debug mode without actually performing any operations on live issues.
    debug-only: # optional, default is false
    # The order to get issues or pull requests. Defaults to false, which is descending.
    ascending: # optional, default is false
    # Delete the git branch after closing a stale pull request.
    delete-branch: # optional, default is false
    # The date used to skip the stale action on issue/pull request created before it (ISO 8601 or RFC 2822).
    start-date: # optional, default is 
    # The assignees which exempt an issue or a pull request from being marked as stale. Separate multiple assignees with commas (eg. "user1,user2").
    exempt-assignees: # optional, default is 
    # The assignees which exempt an issue from being marked as stale. Separate multiple assignees with commas (eg. "user1,user2"). Override "exempt-assignees" option regarding only the issues.
    exempt-issue-assignees: # optional, default is 
    # The assignees which exempt a pull request from being marked as stale. Separate multiple assignees with commas (eg. "user1,user2"). Override "exempt-assignees" option regarding only the pull requests.
    exempt-pr-assignees: # optional, default is 
    # Exempt all issues and pull requests with assignees from being marked as stale. Default to false.
    exempt-all-assignees: # optional, default is false
    # Exempt all issues with assignees from being marked as stale. Override "exempt-all-assignees" option regarding only the issues.
    exempt-all-issue-assignees: # optional, default is 
    # Exempt all pull requests with assignees from being marked as stale. Override "exempt-all-assignees" option regarding only the pull requests.
    exempt-all-pr-assignees: # optional, default is 
    # Exempt draft pull requests from being marked as stale. Default to false.
    exempt-draft-pr: # optional, default is false
    # Display some statistics at the end regarding the stale workflow (only when the logs are enabled).
    enable-statistics: # optional, default is true
    # A comma delimited list of labels to add when a stale issue or pull request receives activity and has the stale-issue-label or stale-pr-label removed from it.
    labels-to-add-when-unstale: # optional, default is 
    # A comma delimited list of labels to remove when a stale issue or pull request receives activity and has the stale-issue-label or stale-pr-label removed from it.
    labels-to-remove-when-unstale: # optional, default is 
    # Any update (update/comment) can reset the stale idle time on the issues and pull requests.
    ignore-updates: # optional, default is false
    # Any update (update/comment) can reset the stale idle time on the issues. Override "ignore-updates" option regarding only the issues.
    ignore-issue-updates: # optional, default is 
    # Any update (update/comment) can reset the stale idle time on the pull requests. Override "ignore-updates" option regarding only the pull requests.
    ignore-pr-updates: # optional, default is 
    - name: Download a Build Artifact
  uses: actions/download-artifact@v2.1.0
  with:
    # Artifact name
    name: # optional
    # Destination path
    path: # optional
    - name: First interaction
  uses: actions/first-interaction@v1.1.0
  with:
    # Token for the repository. Can be passed in using {{ secrets.GITHUB_TOKEN }}
    repo-token: 
    # Comment to post on an individual's first issue
    issue-message: # optional
    # Comment to post on an individual's first pull request
    pr-message: # optional

