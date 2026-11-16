# .github

Organization defaults for [Albino Geek Services Ltd.](https://albinogeek.com/) on GitHub.

GitHub applies the community health files here (`CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`) to every org repo that has none of its own. [`profile/README.md`](profile/README.md) is the org profile shown at github.com/Albino-Geek-Services, so this file is only about the repo.

Edits go through a pull request or a direct commit; there is nothing to build. A pre-commit hook scans staged changes with gitleaks (`lefthook install` once after cloning). CI runs CodeQL, dependency review and OpenSSF Scorecard.

Licensed Apache-2.0, see [LICENSE](LICENSE).
