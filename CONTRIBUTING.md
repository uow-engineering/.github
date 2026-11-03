# Contributing

Write things down so the next person doesn't have to ask: comments in the code, clear commit messages, and a README that's still true. Small fixes are welcome, and you don't need to know git well to make one.

## Setup
Clone the repo to a normal local folder (not one synced to SharePoint, OneDrive may also cause issues). The project README says how to get it running.

## Making changes
- **Maintainers:** commit straight to `main`.
- **Everyone else:** work on your own branch, push it, open a pull request, and a maintainer will merge it. Delete the branch afterwards.
- Commit often, with a message that says what and why.

```bash
git checkout -b short-description
```

## Issues
Record known problems and to-dos in the file header. If the repo uses GitHub Issues, use those instead.

## Versions
`v[major].[minor].[patch]`, set by tagging on GitHub. Not in the code.

| Part | Bump when |
|------|-----------|
| patch | a tagged batch of fixes or tweaks |
| minor | a new feature |
| major | a milestone: done for now, nothing big planned |

Tag after a batch of commits:
```bash
git tag -a v1.2.3 -m "What changed"
git push --tags
```

## File header
Put this at the top of each main file and keep it current.
```cpp
/*
 * [Project Name]
 * Status: [e.g. In development / Deployed on X]
 * Last Updated: YYYY-MM-DD
 * Updated By: [Name]
 * Hardware: [BOM link, or key parts]
 * Notes: [known issues, to-dos]
 * Issues: github.com/uow-engineering/[repo]/issues
 */
```
