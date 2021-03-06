## Supported Operations

### create a release

```
  - uses: jikuma/githubaction@v0.4.0-alpha
      with:
        operation: 'create a release'
        repo-token: ${{ secrets.GITHUB_TOKEN }}
        release_title: 'Release from Test'
        release_note: 'Release created from commit ${{ github.sha }}'
        asset_filepath: './CHANGELOG.md'
        tag_name: v0.1.GITHUB_SHORT_SHA
  - uses: jikuma/githubaction@v0.4.0-alpha
      with:
        operation: 'upload an asset to a release'
        repo-token: ${{ secrets.GITHUB_TOKEN }}
        asset_filepath: './CHANGELOG.md'
        tag_name: v0.1.GITHUB_SHORT_SHA
```



## Contribution

See the walkthrough located [here](https://github.com/actions/typescript-action).

To see the sample usecase refer repositoty [jikuma/githubactiontest](https://github.com/jikuma/githubactiontest/blob/master/.github/workflows/blank.yml)

In addition to walking your through how to create an action, it also provides strategies for versioning, releasing and referencing your actions.


