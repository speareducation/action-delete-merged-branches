# action-delete-merged-branches
Removes merged branches from the git repository

Example:
```
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
        with:
          fetch-depth: 0

      - uses: speareducation/action-delete-merged-branches
        with:
          branch-filter: releases/sandbox/.*
```

