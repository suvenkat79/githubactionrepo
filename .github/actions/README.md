# Configure AWS Credentials Action

This action configures AWS credentials for use in GitHub Actions workflows.

## Inputs

| Input | Description | Required | Default |
| ----- | ----------- | -------- | ------- |
| `aws-access-key-id` | AWS Access Key ID | Yes | N/A |
| `aws-secret-access-key` | AWS Secret Access Key | Yes | N/A |
| `aws-region` | AWS Region | Yes | us-east-1 |

## Example Usage

```yaml
- name: Configure AWS
  uses: ./.github/actions/configure-aws-credentials
  with:
    aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
    aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    aws-region: us-east-1
