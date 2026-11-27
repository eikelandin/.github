# Contributing

How to report a problem and propose a change in a public repository of [@eikelandin](https://github.com/eikelandin) that has no `CONTRIBUTING.md` of its own. The repository's README names its setup and checks.

## Report a problem or ask for something

- Open an issue with the bug report or feature request form, and start with the plain-words field: what is wrong or wanted, for someone who does not know the code.
- Report a vulnerability privately, as the [security policy](https://github.com/eikelandin/.github/blob/main/SECURITY.md) describes, never as an issue.

## Propose a change

1. For more than a small fix, open an issue first, so the approach is agreed before the work starts.
2. Branch from the default branch and open the pull request against it. Say what changes, why, and how you checked it.
3. Write the pull request title in [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) form, for example `fix(api): reject an empty name`. Pull requests are squash-merged, so the title becomes the commit message.
4. Sign your commits with an SSH or GPG key ([signing commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits)).
5. The repository's tests and checks pass before review. A change in behavior comes with a test that fails without it.

A pull request is accepted when its checks pass, its review threads are resolved and the maintainer accepts the change. A pull request that adds scope nobody agreed on, or that has no reply for 30 days after a review, may be closed with a note.

## Dependencies

- Selection: prefer the language's standard library or the platform, then a dependency the repository already uses, then a maintained, widely used package with a license compatible with the repository's. Each new dependency is named and justified in the pull request.
- Sources: packages come from the ecosystem's official registry through the repository's package manager, with the lockfile committed. GitHub Actions are pinned to a full commit SHA.
- Tracking: Dependabot opens version and security updates; they are reviewed and pass the same checks as any other change.

## Governance

The maintainer, [@eikelandin](https://github.com/eikelandin), owns every repository, holds admin access and is the only person who merges. No one else has write access. Bots and GitHub Apps installed on a repository (for example Dependabot) open or comment on pull requests; their changes go through the same pull request rules and checks.

## License

A contribution is licensed under the license of the repository it goes into. There is no contributor license agreement (CLA).
