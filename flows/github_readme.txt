1. Copy the variables from github_env.yaml into <sequor_env_dir>/variables.yaml and fill in the values of the variables.
2. You can find instructions on generating github_bearer_token in our quick guide where we use GitHub REST API as examples
3. Here is a link to the GitHub REST API docs https://docs.github.com/en/rest

github_repo_health flow is the example from our quickstart extended with the last "http_request: delete_gist" at the end to delete the created gist. Comment out this operation if you want to see the created gist.
flows/github_fetch_issues.yaml flow is an extended version of "http_request: get_issues" operation that demostrate how to handle pagination.