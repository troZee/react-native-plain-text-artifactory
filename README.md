# react-native-plain-text visual baselines

Canonical expected images for the visual regression tests in
[`react-native-plain-text`](https://github.com/troZee/react-native-plain-text).

The library repository pins this repository as its `baselines/` Git submodule.
Each platform directory is further separated by the exact device profile used
to capture it.

Only reviewed expected images belong here. Actual captures, image diffs,
comparison reports, and native logs are temporary CI artifacts and must not be
committed.

## Updating baselines

1. Generate candidate images from the canonical simulator or emulator
   environment.
2. Open and merge a pull request in this repository.
3. Update the `baselines/` submodule pointer in the corresponding library pull
   request.
4. Cross-link both pull requests so reviewers can inspect the image changes.

Do not force-push or rewrite commits referenced by the library repository.
