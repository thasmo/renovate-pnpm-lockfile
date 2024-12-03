# 32552

## Current behavior

Any successive renovate run (except the initial run, which creates a PR) 
**will not update** the version of the dependency in the
**`pnpm-lockfile.yaml`** file, and therefore will be
**out of sync with the PR title**.

* PR Title: `chore(deps): update dependency knip to v5.39.1`
* File Change: `knip@5.39.0:`

## Expected behavior

Any successive renovate run (including the initial run, which creates a PR)
**will update** the version of the dependency in the `pnpm-lockfile.yaml` file,
and therefore will be **in sync** with the PR title.

* PR Title: `chore(deps): update dependency knip to v5.39.1`
* File Change: `knip@5.39.1:`

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/32552
