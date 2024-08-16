# joshuaavalon/action-npm-publish

## Usage

```yaml
name: release
on:
  push:
    branches:
      - master
jobs:
  release-package:
    permissions:
      id-token: write
    uses: joshuaavalon/publish-npm@v1
    with:
      workspace: "@joshuaavalon/workspace-pkg"
      npm-token: ${{ secrets.NPM_TOKEN }}
```
