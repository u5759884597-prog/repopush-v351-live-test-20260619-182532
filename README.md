# RepoPush Demo

RepoPush Demo turns one product brief into a review-ready GitHub documentation pack and safe PR push.

![RepoPush Generated](https://img.shields.io/badge/docs-RepoPush%20generated-informational) ![License](https://img.shields.io/badge/license-MIT-blue)

**What it is:** RepoPush Demo helps solo founders, developer advocates, open-source maintainers solve: Teams often ship repositories with incomplete README files, missing support paths, inconsistent roadmap claims, and issue templates that slow down triage.

**Fast path:** install with `pip install repopush` and complete the quickstart below in 4 steps.

![RepoPush dashboard](<https://example.com/assets/repopush-dashboard.png>)

## Why

Teams often ship repositories with incomplete README files, missing support paths, inconsistent roadmap claims, and issue templates that slow down triage.

Use RepoPush Demo when you need a documented, supportable workflow for solo founders, developer advocates, open-source maintainers without mixing launch-ready claims with beta or roadmap work.

## Install

```bash
pip install repopush
python src/repopush.py audit --input sample_product_brief.json
```

## Quickstart

1. Create a product brief JSON file.
2. Run `python src/repopush.py compile --input sample_product_brief.json --platform github --out output_pack`.
3. Run `python src/repopush.py validate --pack output_pack/github`.
4. Run a dry-run install plan before opening a PR.

## Features

### Launch features

- **GitHub Pack compiler** — Available now. Generates README, support, security, contributing, docs, and issue-template files from one product brief.
- **ClaimMatrix consistency checks** — Available now. Tracks launch, beta, roadmap, and deprecated claims across generated files.

### Beta features

- **Repository topic suggestions** — Beta. Suggests GitHub topics based on product type and generated content.

### Roadmap preview

- **GitHub Repo Importer** — Planned. Will inspect an existing repository and infer missing product brief fields.

## Examples

- Compile a GitHub Pack from a SaaS product brief.
- Validate README sections and issue form YAML before installing.
- Generate a dry-run install plan for an existing repository.

## Limitations

- ClaimMatrix consistency checks: Requires accurate feature status in the source brief.
- Repository topic suggestions: Topics are suggestions and must be applied manually.
- GitHub Repo Importer: Importer interface is reserved in MVP v3 RC and is not active by default.
- Legacy HTML exporter: Not part of the GitHub PR installer path.
- Beta features are marked as beta and should be validated before production use.
- Planned roadmap items remain planned and are not represented as launch functionality.

## FAQ

### Does RepoPush push directly to main?

No. The installer refuses default-branch writes and only creates or updates a dedicated RepoPush branch.

### Can it install GitHub workflows?

No. Workflows are intentionally excluded from the default MVP v3 RC pack.

### What happens if a file was edited by a maintainer?

The diff plan marks the file for manual review and does not silently overwrite it.

## Links

- Website: https://repopush.com
- Repository: https://github.com/example/repopush-demo
- Support: see [SUPPORT.md](SUPPORT.md)
- Security: see [SECURITY.md](SECURITY.md)

## Contributing

Contributions are welcome through issues and pull requests. Start with [CONTRIBUTING.md](CONTRIBUTING.md) and use the provided issue forms so maintainers can triage quickly.

## License

This project is distributed under the MIT license. See [LICENSE](LICENSE) for details.
