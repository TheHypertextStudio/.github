# Contributing to Hypertext Studio projects

This guide applies to every Hypertext Studio repository that does not have its own `CONTRIBUTING.md`. The Studio is one maintainer, so a focused change with a clear description gets reviewed soonest.

## What you can do without Studio access

You never need a Studio account, a Studio email address or access to Studio infrastructure to contribute.

- **Report a bug or propose a change.** Open an issue with the bug report or proposal form when the repository accepts issues. For a large change, open a proposal first so you know the direction is wanted before you spend time on it.
- **Build and test the project.** Follow the quickstart in the repository's `docs/DEVELOPMENT.md`. It lists the toolchain and the commands that work on a fresh clone with no Studio credentials. If a step asks you to sign in to a Studio account, the quickstart is wrong: open an issue.
- **Open a pull request from your fork.** Keep each pull request to one change, and fill in the pull request outline.
- **Report a vulnerability privately.** Follow the [security policy](https://github.com/TheHypertextStudio/.github/blob/main/SECURITY.md). Never put security details in a public issue.

## How your pull request is checked

Studio machines never run a pull request from a fork directly, so the checks don't start on your pull request itself. A maintainer reads your change first, then pushes your commits, with your authorship, to a branch in the repository, where the repository's protected checks run. They are the same checks a maintainer's change must pass: the tests, formatting, commit messages and documentation links.

The repository's Git hooks are for maintainers; leave them uninstalled. The checks on your change are what decide.

When a check fails, its log names the problem and the fix. You can push more commits to your branch, and the maintainer runs the checks on them again. A maintainer may also apply formatting or reword a commit message while rebasing your branch, and keeps your authorship when doing so.

## Commit messages

Write each commit message as `type(scope): summary`, for example `fix(sync): retry an interrupted upload`.

- `feat` adds something a person using the product can now do. `fix` corrects behavior that person would notice. Everything else is `chore`.
- The scope names the part of the product the change affects. Use a scope that already appears in the repository's history.
- Describe what changed for the person using the product, not which files moved.

If an AI tool wrote part of your change, end the commit message with a `Co-authored-by:` trailer naming that tool, in the form the tool documents.

## What only maintainers do

Some work needs Studio credentials or carries responsibility for people who use the products, so only a maintainer does it:

- merging pull requests and changing protected branches,
- releasing, signing and publishing builds, and deploying services,
- reading or changing Studio infrastructure, staging and production data, and credentials,
- triaging private vulnerability reports and publishing advisories,
- running the checks on a contributor's change.

If your change needs one of these steps, say so in the pull request. The maintainer completes it after review.

## Licensing of contributions

Each repository states its license in its README and `LICENSE` file. Under GitHub's Terms of Service, a contribution you submit to a repository is offered under that repository's license. Do not submit code you do not have the right to license that way.

## Conduct

Everyone taking part follows the [code of conduct](https://github.com/TheHypertextStudio/.github/blob/main/CODE_OF_CONDUCT.md).
