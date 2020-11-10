# Contributing

Thank you for your interest in Peaks.js!

We love hearing feedback from people who use our software, so if you build something interesting using this library, please let us know.

Contributions are welcomed and encouraged. If you're thinking of fixing a bug or writing a new feature, please first read the following guidelines.

## Making changes

* Before creating a pull request, we prefer that you first discuss the change you wish to make, either by raising an issue, or contacting us directly, e.g, [by email](mailto:irfs@bbc.co.uk).

* Please check our [development plan](https://github.com/bbc/peaks.js/projects/1), which shows the current and planned changes.

* If we agree with your feature proposal, we'll work with you to develop and integrate the feature. But please bear with us, as we may not always be able to respond immediately.

* Please avoid making commits directly to your copy of the `master` branch. This branch is reserved for aggregating changes from other people, and for mainline development from the core contributors. If you commit to `master`, it's likely that your local fork will diverge from the [upstream repository](https://github.com/bbc/peaks.js).

* Before working on a change, please ensure your local fork is up to date with the code in the upstream repository, and create a [feature branch](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow) for your changes.

* Please don't change the `version` field in [package.json](https://github.com/bbc/peaks.js/blob/master/package.json), or update [CHANGELOG.md](https://github.com/bbc/peaks.js/blob/master/CHANGELOG.md). We'll do that when [preparing a new release](#preparing-a-new-release).

* Please follow the existing coding conventions, and ensure that there are no linting errors (`npm run lint`). The eslint config doesn't specify all our coding conventions, so please try to be consistent. (We realise there are some inconsistencies in the codebase already, we're slowly working to resolve them.)

* For commit messages, please follow [these guidelines](https://chris.beams.io/posts/git-commit/), although we're not fussy about use of imperative mood vs past tense. In particular, avoid commit messages that include [Angular-style metadata](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit-message-header).

* Please add test cases for your feature, and ensure all tests are passing (`npm run test`).

* When merging a feature branch, core contributors may choose to squash your commits, so that the feature is merged as a single logical change.

### Preparing a new release

When it's time to publish a new release version, e.g,. to npm, create a single commit on `master` with the following changes only:

* Increment the `version` field in [package.json](https://github.com/bbc/peaks.js/blob/master/package.json)

* Describe the new features in this release in [CHANGELOG.md](https://github.com/bbc/peaks.js/blob/master/CHANGELOG.md)

Tag this commit using the form `vX.Y.Z` and push the commit using `git push origin master --tags`.
