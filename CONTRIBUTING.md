# Contributing to horizons-api

Thanks for your interest in contributing to horizons-api!

Contained below are the setup, guidelines, and expectations
of any contributions submitted to this package.

## Getting Started

### Requirements

- Have Git installed on your local computer
- Have Node installed on your local computer
  - Recommend using nvm for managing Node versions
  - Recommend using Node 18+

### Setup

The repository must be forked to your own account, then you can run the following commands to get started:

```terminal
git clone https://github.com/{account}/horizons-api.git
cd horizons-api
npm install
```

## Development

The following is expected of all development that takes place within this package.

### Test Driven Development (TDD)

All development done within this package should follow the practices of TDD as follows:

- Write precise tests - Write tests that will verify the exact functionality that you are trying to implement, these tests will likely fail as the solution has not yet been coded.
- Correct the code - Once the tests are failing, make the necessary changes required to get the test to pass
- Refactor - Once your tests are passing, look for ways to optimize the code, these changes should not break any tests or change the overall functionality of the code

### Linting

This package is being linted using ESLint and Prettier to help keep the coding consistent and readable.
This linting is also included in the pipeline and will fail if not completed successfully.
There are plugins that can help automatically enforce the linting defined in different IDEs, but if you do not want to use those (or they aren't working), you can use the following commands to find and fix any linting issues within the project:

```terminal
# Find any linting issues
npm run lint

# Resolve all fixable issues
npm run lint -- --fix
```

### Commit Message Formatting

`semantic-release` uses commit messages to determine if a release is necessary when the pipeline is run.
Therefore, the commit messages need to have a specific structure so that the release process can determine if a new release is required.

The formatting of the commit must follow:

```text
<type>(optional scope): summary
```

#### **Type**

Used to determine if a release is necessary, must be one of the following values:

| Type | Description | Release |
|:----:|:-----------:|:-------:|
|**build**|Changes that affect the build system or external dependencies|No Release|
|**chore**|Automated changes to project|No Release|
|**ci**|Changes to CI configuration files and scripts|No Release|
|**docs**|Changes to documentation|No Release|
|**feat**|Implementation of a new feature|Minor/Feature Release|
|**fix**|Changes that fix bugs|Patch/Fix Release|
|**perf**|Changes to improve performance|Major/Breaking Release|
|**refactor**|Code change that does not fix a bug or add a feature|No Release|
|**test**|Adding or updating tests|No Release|

> *[Updates](https://github.com/semantic-release/semantic-release#commit-message-format) can be made to what types trigger releases in `release.config.js`*

#### **Scope** (optional)

Name of the component affected

#### **Summary**

Brief description of the update made

## Pull Requests

Use the pull request template to help give context to the proposed changes that you are making and help link it to an open issue.

## Issues

Please use the issue template that most closely matches what you are looking to provide.
If none align with your intent, then submit a feature request issue and we can have additional discussion within the issue.
