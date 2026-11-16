# AGENTS.md

Org defaults for Albino Geek Services Ltd. GitHub treats this repo specially: `profile/README.md` is the org landing page, and the community health files here apply to every repo in the org that has none of its own.

## Layout

- `profile/README.md`: the public org profile. Offers and prices live on [albinogeek.com](https://albinogeek.com/); the profile points there and does not restate them.
- `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`: org-wide defaults.
- `.github/workflows/`: CodeQL, dependency review and OpenSSF Scorecard. `.github/dependabot.yml` covers the workflow actions.
- `lefthook.yml` and `.gitleaks.toml`: the pre-commit secret scan.

## Verify

There is no build or test suite. Before a commit, run `gitleaks git --redact --no-banner` and read the rendered `profile/README.md` for broken links.

## Invariants

- Public repo: nothing private, no client names, no pricing that is not already on the site.
- Product repos stay private; the profile does not catalogue them.
- Workflow actions are pinned to a full commit SHA.
