# Contributing

Thanks for helping. This guide covers every repository in the organisation; a repository's own CONTRIBUTING file adds project-specific steps.

## Before you start

- Read the [Code of Conduct](CODE_OF_CONDUCT.md) and the [AI policy](AI_POLICY.md).
- For anything larger than a bug fix, open an issue or ask on Discord first. Balance and progression changes need the author's approval.

## Pull requests

1. Fork, create a branch from `main`, keep one topic per PR.
2. Match the style of the surrounding code; run `./gradlew spotlessApply` where the project has it.
3. Every new machine, item or recipe ships with names in **en_us, pt_br and zh_cn**.
4. Add or update GameTests for what you changed. A new multiblock needs at least a "forms" test and a negative test (it must not form or run when it should not).
5. Run `./gradlew build runGameTestServer` and say in the PR how you tested in game.
6. Commit messages and changelog entries are written in English.

## Releases

- `main` builds nightly packages for testers.
- Tagged versions follow `X.Y.Z-dev-N`, `-pre-N`, `-alpha`, `-beta`; only beta and later are published as stable.
