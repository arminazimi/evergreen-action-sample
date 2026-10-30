# evergreen-action-sample

A tiny repository that shows the [Evergreen](https://github.com/arminazimi/evergreen) GitHub Action working on a schedule:

- **Fix pull request.** `fix-pr: "true"` keeps one pull request on `evergreen/fixes` with every deterministic fix (here, the end-of-life base image in `Dockerfile`).
- **Tracking issue.** `tracking-issue: "true"` keeps one issue that lists what is past or near end of life, including the deprecated `request` dependency.

The workflow is `.github/workflows/evergreen.yml`; it runs every Monday and can be started by hand from the Actions tab. Leave the fix pull request open to keep the demo alive. Docs: [GitHub Action](https://github.com/arminazimi/evergreen/blob/main/docs/GITHUB_ACTION.md).
