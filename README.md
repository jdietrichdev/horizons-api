# horizons-api

Template repsitory for creating a deployable NPM package

## Getting Started

Guide for getting this template repository set up for usage with your own NPM package

### Defining Contributions

Use the [CONTRIBUTING.md](./CONTRIBUTING.md) file to define how contributions to your project should be made.

This file should include:

- Instructions for setting up the project locally
- Expectations for development practices while updating the codebase
- Expectations for issues and pull requests created within the project

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
