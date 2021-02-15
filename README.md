# gipht-action
An action to present gifs.

## Setup

```
name: "Gipht Me"
on:
  issue_comment:
    types: [created]

jobs:
  comment-run:
    runs-on: ubuntu-latest
    steps:
      - uses: bdougie/gipht-action@main
        env:
          GIPHY_TOKEN: ${{ secrets.GIPHY_TOKEN }} // generate at https://developers.giphy.com/
          GITHUB_TOKEN: ${{ secrets.BDOUGIE_TOKEN }} // must be generate and provide access to the repo's issue.
```
