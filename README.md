# Critical Dependabot Jira
Create a jira ticket of issue type **Bug** when a critical dependabot PR is created in the repository.

# Usage
See [action.yml](https://github.com/Orfium/critical-dependabot-jira/blob/master/action.yml).

## Inputs
The action needs a series of inputs to be set in order to function properly.

| Item            | Description                                                                                                                        | Default             |
|-----------------|------------------------------------------------------------------------------------------------------------------------------------|---------------------|
| jira_base_url   | The base url of jira.                                                                                                              | -                   |
| jira_user_email | The email of jira user to open the bug.                                                                                            | -                   |
| jira_project    | The jira project that the bug will be opened.                                                                                      | -                   |
| jira_issue_type | The jira ticket issue type.                                                                                                        | Bug                 |
| jira_label      | The jira ticket label.                                                                                                             | dependabot-critical |
| cvss_threshold  | The [CVSS](https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System) threshold that you want to trigger the bug creation. | 9.0                 |

### Secrets needed
The repository needs two secrets, the `pat_token` which is a
[Github Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
with the `repo.public_repo` scope and the `jira_api_token` which is a [Jira API Token](https://id.atlassian.com/manage-profile/security/api-tokens).

## Outputs
Nothing to output.

## Example of usage
TBA


