[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/nodes-app/action-google-credentials)

# action-google-credentials

This action sets up GCP credentials for use by subsequent steps.

## Usage

```yml
- name: Set Up GCP Credentials
  uses: nodes-app/action-google-credentials@v1
  with:
    service-account-key: ${{ secrets.GCP_SERVICE_ACCOUNT_KEY }}

- name: Use GCP Credentials
  run: |
    echo "Path to credentials: $GOOGLE_APPLICATION_CREDENTIALS"
```
