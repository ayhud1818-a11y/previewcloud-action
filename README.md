# PreviewCloud GitHub Action

[![GitHub release](https://img.shields.io/github/release/previewcloud/action.svg)](https://github.com/previewcloud/action/releases)

A simple GitHub Action to create and manage preview environments for your pull requests.

## Usage

```yaml
- uses: previewcloud/action@v1.0.0
  with:
    api_key: ${{ secrets.PREVIEWCLOUD_API_KEY }}
    pr_number: ${{ github.event.pull_request.number }}
    branch: ${{ github.head_ref }}
    commit_sha: ${{ github.sha }}
    repository: ${{ github.repository }}