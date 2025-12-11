# Releasing

This project uses GitHub Actions to publish to npm. The publish workflow runs when a tag with the format `v*` is pushed.

## Steps to cut a release

1. **Apply the changesets**. Run `pnpm changeset version` and review the changes.
2. **Commit and tag**. `git commit -m X.Y.Z && git tag vX.Y.Z`
3. **Push and push tags**. `git push && git push --tags`
4. **Create a GitHub release**. Go to the [tags](https://github.com/slippy-lint/slippy/tags) page and create a release using the new tag.
