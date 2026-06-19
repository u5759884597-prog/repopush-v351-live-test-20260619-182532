# FAQ

### Does RepoPush push directly to main?

No. The installer refuses default-branch writes and only creates or updates a dedicated RepoPush branch.

### Can it install GitHub workflows?

No. Workflows are intentionally excluded from the default MVP v3 RC pack.

### What happens if a file was edited by a maintainer?

The diff plan marks the file for manual review and does not silently overwrite it.

## Troubleshooting

Open a question issue with version information, reproduction steps, and redacted logs when the FAQ does not resolve the problem.
