# Github Issue Action

This action opens a new github issue.

## Inputs

### `token`

**Required** Github Token.

### `title`

**Required** Issue title.

### `body`

Issue body.

### `assignees`

Issue assignees. Passed as a formatted multi-line string using the | character.

## Outputs

### `issue`

The issue object as a json string.

## Example usage

```yaml
uses: alialaa/issue-action@v1
with:
  token: ${{ secrets.GITHUB_TOKEN }}
  title: Some Issue Title
  body: Some Issue Body
  assignees: |
    alialaa
    alialaa17
```
