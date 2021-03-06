# Ignition Test : Testing framework for Ignition

Naming ideas:

  1. simtest
  2. gztest
  3. behavior...
  4. hygiene....
  5. genie, jinn
  6. audition
  7. appraise
  8. exam
  8. quiz
  9. insight
  10. scenario 

**Maintainer:** nate AT openrobotics DOT org

[![GitHub open issues](https://img.shields.io/github/issues-raw/ignitionrobotics/ign-test.svg)](https://github.com/ignitionrobotics/ign-test/issues)
[![GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/ignitionrobotics/ign-test.svg)](https://github.com/ignitionrobotics/ign-test/pulls)
[![Discourse topics](https://img.shields.io/discourse/https/community.gazebosim.org/topics.svg)](https://community.gazebosim.org)
[![Hex.pm](https://img.shields.io/hexpm/l/plug.svg)](https://www.apache.org/licenses/LICENSE-2.0)

Build | Status
-- | --
Test coverage | [![codecov](https://codecov.io/gh/ignitionrobotics/ign-test/branch/main/graph/badge.svg)](https://codecov.io/gh/ignitionrobotics/ign-test)
Ubuntu Bionic | [![Build Status](https://build.osrfoundation.org/buildStatus/icon?job=ignition_test-ci-main-bionic-amd64)](https://build.osrfoundation.org/job/ignition_test-ci-main-bionic-amd64)
Homebrew      | [![Build Status](https://build.osrfoundation.org/buildStatus/icon?job=ignition_test-ci-main-homebrew-amd64)](https://build.osrfoundation.org/job/ignition_test-ci-main-homebrew-amd64)
Windows       | [![Build Status](https://build.osrfoundation.org/job/ign_test-ci-win/badge/icon)](https://build.osrfoundation.org/job/ign_test-ci-win/)

Ignition Test, a component of [Ignition
Robotics](https://ignitionrobotics.org), provides testing framework for
robot applications.

# Table of Contents

[Features](#features)

[Install](#install)

[Usage](#usage)

[Documentation](#documentation)

[Testing](#testing)

[Folder Structure](#folder-structure)

[Code of Conduct](#code-of-conduct)

[Contributing](#code-of-contributing)

[Versioning](#versioning)

[License](#license)

# Features

Ignition Test provides a testing framework.

# Install

See the [installation tutorial](https://ignitionrobotics.org/api/test/0.1/install.html).

# Usage

Please refer to the [examples directory](https://github.com/ignitionrobotics/ign-test/blob/main/examples/).

# Documentation

API and tutorials can be found at [https://ignitionrobotics.org/libs/test](https://ignitionrobotics.org/libs/test).

You can also generate the documentation from a clone of this repository by following these steps.

1. You will need Doxygen. On Ubuntu Doxygen can be installed using

    ```
    sudo apt-get install doxygen
    ```

2. Clone the repository

    ```
    git clone https://github.com/ignitionrobotics/ign-test
    ```

3. Configure and build the documentation.

    ```
    cd ign-test; mkdir build; cd build; cmake ../; make doc
    ```

4. View the documentation by running the following command from the build directory.

    ```
    firefox doxygen/html/index.html
    ```

# Testing

Follow these steps to run tests and static code analysis in your clone of this repository.

1. Follow the [source install instruction](https://ignitionrobotics.org/libs/test#source-install).

2. Run tests.

    ```
    make test
    ```

3. Static code checker.

    ```
    make codecheck
    ```

# Folder Structure

Refer to the following table for information about important directories and files in this repository.

```
ign-test
????????? examples                 Example programs.
????????? include/ignition/test   Header files.
????????? src                      Source files and unit tests.
????????? test
???    ????????? integration         Integration tests.
???    ????????? performance         Performance tests.
???    ????????? regression          Regression tests.
????????? tutorials                Tutorials, written in markdown.
????????? Changelog.md             Changelog.
????????? CMakeLists.txt           CMake build script.
```
# Contributing

Please see
[CONTRIBUTING.md](https://ignitionrobotics.org/docs/all/contributing).

# Code of Conduct

Please see
[CODE_OF_CONDUCT.md](https://github.com/ignitionrobotics/ign-test/blob/main/CODE_OF_CONDUCT.md)

# Versioning

This library uses [Semantic Versioning](https://semver.org/).
Additionally, this library is part of the
[Ignition project](https://ignitionrobotics.org) which periodically
releases a versioned set of compatible and complimentary libraries. See the
[Ignition website](https://ignitionrobotics.org) for version and
release information.

# License

This library is licensed under
[Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0).
See also the
[LICENSE](https://github.com/ignitionrobotics/ign-test/blob/main/LICENSE)
file.

