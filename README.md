# Use branch name on GitHub actions

Convenience action for using current branch name.

## Usage
```
name: build
on: push

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
    - run: npm ci
    - uses: jason2866/branch-name@master
    # Use branch name for whatever purpose
    - run: echo ${BRANCH_NAME}
```
