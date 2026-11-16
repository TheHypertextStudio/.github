# Hypertext Studio community defaults

GitHub shows the files in this repository in every Hypertext Studio repository that does not carry its own file of the same kind. A contributor who opens a repository's Contributing, Security or Code of conduct link reads the text below.

| File                               | What a visitor sees                                                                         |
| ---------------------------------- | ------------------------------------------------------------------------------------------- |
| `CONTRIBUTING.md`                  | How to propose a change without Studio access, and which work only maintainers do.          |
| `SECURITY.md`                      | How to report a vulnerability privately through GitHub.                                     |
| `CODE_OF_CONDUCT.md`               | The Contributor Covenant, adopted by reference, with the Studio as the enforcement contact. |
| `SUPPORT.md`                       | Where to ask a question and what support to expect.                                         |
| `.github/ISSUE_TEMPLATE/`          | The bug report and proposal forms, and the links shown before a new issue.                  |
| `.github/pull_request_template.md` | The pull request outline.                                                                   |

## How GitHub applies these files

A repository's own file always wins. When a repository has a `CONTRIBUTING.md`, for example, GitHub shows that file and ignores the default here. Issue templates are replaced as a whole folder: a repository with any valid file in its own `.github/ISSUE_TEMPLATE/` uses none of the default forms.

The defaults do not appear in a repository's file list, history, clones or downloads. GitHub reads them only when it renders the repository on the website.

Each repository carries its own license, `CODEOWNERS`, workflows and development guide.
