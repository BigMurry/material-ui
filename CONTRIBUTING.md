# Contributing

If you're reading this, you're awesome! Thank you for helping us make this project great and being a part of the Material-UI community. Here are a few guidelines that will help you along the way.

## Asking Questions

For how-to questions and other non-issues, please use [StackOverflow](http://stackoverflow.com/questions/tagged/material-ui) or [Gitter](https://gitter.im/callemall/material-ui) chat instead of Github issues. There is a StackOverflow tag called "material-ui" that you can use to tag your questions.

## Opening an Issue

If you think you have found a bug, or have a new feature idea, please start by making sure it hasn't already been [reported or fixed](https://github.com/callemall/material-ui/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aclosed). You can search through existing issues and PRs to see if someone has reported one similar to yours.

Next, create a new issue that briefly explains the problem, and provides a bit of background as to the circumstances that triggered it, and steps to reproduce it.

For code issues please include:
* Material-UI version
* React version
* Browser version
* A code example or link to a repo, gist or running site.

For visual or layout problems, images or animated gifs can help explain your issue.
It's even better with a live reproduction test case. Have a look at the [`ISSUE_TEMPLATE.md`](https://raw.githubusercontent.com/callemall/material-ui/master/.github/ISSUE_TEMPLATE.md) file for a live playground example.

For feature requests please include a link to the relevant section of Material Design spec, or a screenshot.

### Issue Guidelines

Please begin the title with '[ComponentName]' where appropriate, and use a succint description. "doesn't work" doesn't help others find similar issues.

Please don't group multiple topics into one issue, but instead each should be its own issue.

And please don't just '+1' an issue. It spams the maintainers and doesn't help move the issue forward.

## Submitting a Pull Request

Material-UI is a community project, so pull requests are always welcome, but before working on a large change, it is best to open an issue first to discuss it with the maintainers.

When in doubt, keep your pull requests small. To give a PR the best chance of getting accepted, don't bundle more than one feature or bug fix per pull request. It's always best to create two smaller PRs than one big one.

As with issues, please begin the title with [ComponentName].

When adding new features or modifying existing, please attempt to include tests to confirm the new behaviour. You can read more about our test setup [here](https://github.com/callemall/material-ui/blob/master/test/README.md).

### Branch Structure

All stable releases are tagged ([view tags](https://github.com/callemall/material-ui/tags)). At any given time, `master` represents the latest development version of the library. Patches or hotfix releases are prepared on an independent branch.

#### `master` is unsafe

We will do our best to keep `master` in good shape, with tests passing at all times. But in order to move fast, we will make API changes that your application might not be compatible with.


## Getting started

Please create a new branch from an up to date master on your fork. (Note, urgent hotfixes should be branched off the latest stable release rather than master)

1. Fork the Material-UI repository on Github
2. Clone your fork to your local machine `git clone git@github.com:<yourname>/material-ui.git`
3. Create a branch `git checkout -b my-topic-branch`
4. Make your changes, lint, then push to github with `git push --set-upstream origin my-topic-branch`.
5. Visit github and make your pull request.

If you have an existing local repository, please update it before you start, to minimise the chance of merge conflicts.
```js
git remote add upstream git@github.com:callemall/material-ui.git
git checkout master
git pull upstream master
git checkout -b my-topic-branch
npm update
```

### Testing the documentation site

The documentation site is built with Material-UI, and contains examples of all the components. To get started:
```js
npm install
cd docs
npm install
npm start
```
You can now access the documentation site [locally](http://localhost:3000).

Test coverage is limited at present, but where possible, please add tests for any changes you make. Tests can be run with `npm run test`.

### Coding style

Please follow the coding style of the current code base. Material-UI uses eslint, so if possible, enable linting in your editor to get realtime feedback. The linting rules are also run when Webpack recompiles your changes, and can be run manually with `npm run lint`.

You can also run linting on a subset of the codebase with `gulp eslint:src`, `gulp eslint:docs` or `gulp eslint:test`. Finally, when you submit a pull request, they are run again by Travis CI, but hopefully by then your code is already clean!

## Roadmap

To get a sense of where Material-UI is heading, or for ideas on where you could contribute, take a look at the [roadmap](https://github.com/callemall/material-ui/blob/master/ROADMAP.md) and the list of [Material Design components](https://github.com/callemall/material-ui/issues/2863).


## License

By contributing your code to the callemall/material-ui GitHub repository, you agree to license your contribution under the MIT license.
