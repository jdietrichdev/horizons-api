# Contributing to horizons-api

Thanks for your interest in contributing to horizons-api!

Contained below are the setup, guidelines, and expectations
of any contributions submitted to this package.

## Setup

## Development

### Test Driven Development (TDD)

All development done within this package should follow the practices of TDD as follows: 

- Write precise tests - Write tests that will verify the exact functionality that you are trying to implement, these tests will likely fail as the solution has not yet been coded.
- Correct the code - Once the tests are failing, make the necessary changes required to get the test to pass
- Refactor - Once your tests are passing, look for ways to optimize the code, these changes should not break any tests or change the overall functionality of the code

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
