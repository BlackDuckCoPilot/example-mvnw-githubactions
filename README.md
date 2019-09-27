# Black Duck CoPilot Gradle/GitHub CI Example

[![Actions](https://github.com/BlackDuckCoPilot/example-mvnw-githubactions/workflows/Java%20CI/badge.svg)](https://github.com/BlackDuckCoPilot/example-mvnw-githubactions/actions?workflow=Java+CI) [![Black Duck Security Risk](https://copilot-test.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-mvnw-githubactions/branches/test/badge-risk.svg)](https://copilot-test.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-mvnw-githubactions/branches/test)

Shows a working setup for using the Black Duck CoPilot integration to analyze the risk of project dependencies

## GitHub CI/CD Setup

The `.github/workflows/workflow.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- name: Upload to CoPilot
      run: bash <(curl -s https://copilot-test.blackducksoftware.com/ci/githubactions/scripts/upload)
```
