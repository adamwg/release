# Crossplane Release Process

This repository contains complete end-to-end process and instructions for how to
release new versions of the core
[Crossplane](https://github.com/crossplane/crossplane) software.

For more information about releasing Crossplane extensions, for example
Providers and Functions, please see the [Crossplane documentation
page](https://docs.crossplane.io/latest/guides/extensions-release-process/).

## tl;dr Process Overview

All the details are available in the template issues linked below, but here is a
summary of the process to understand how it works at a high level:

1. **code freeze**: Merge all completed features and bug fixes into the main
   development branch to begin "code freeze".
1. **update dependencies**: Ensure all dependencies are up to date, especially
   security related updates.
1. **create release branch**: Create a new release branch using the GitHub UI
   for the repo.
1. **publish RC build**: Tag, build, and publish a release candidate (RC) build
   for the community to test and provide feedback on.
1. **fix critical issues**: Triage and fix any critical issues found in the RC
   build and ensure all fixes are backported to the release branch.
1. **publish release build**: Tag, build, and publish the final release build
1. **run docs release**: Run the [release
   process](https://github.com/crossplane/docs/issues/new?assignees=&labels=release&template=new_release.md&title=Release+Crossplane+version...+)
   for [docs.crossplane.io](https://docs.crossplane.io/)
1. **verify**: Verify all artifacts have been published successfully, perform
   sanity testing.
1. **release notes**: Publish well authored and complete release notes on
   GitHub.
1. **announce**: Announce the release on Crossplane social media accounts.

## Detailed Process

The complete step-by-step process to release Crossplane is captured in the below
GitHub issue templates:

* [Major or minor
  release](https://github.com/crossplane/release/blob/main/.github/ISSUE_TEMPLATE/release.md)
* [Patch
  release](https://github.com/crossplane/release/blob/main/.github/ISSUE_TEMPLATE/patch_release.md)

When preparing to run a Crossplane release, open a tracking issue using the
relevant template above, and follow the entire checklist of instructions to
completion.