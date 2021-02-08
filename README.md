# Spout

[![Latest Stable Version](https://poser.pugx.org/guss77/spout-fork/v/stable)](https://packagist.org/packages/guss77/spout-fork)
[![Project Status](https://opensource.box.com/badges/active.svg)](https://opensource.box.com/badges)
[![Build Status](https://travis-ci.com/guss77/spout.svg?branch=master)](https://travis-ci.com/guss77/spout)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/guss77/spout/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/guss77/spout/?branch=master)
[![Code Coverage](https://scrutinizer-ci.com/g/guss77/spout/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/guss77/spout/?branch=master)
[![Total Downloads](https://poser.pugx.org/guss77/spout/downloads)](https://packagist.org/packages/guss77/spout)

Spout is a PHP library to read and write spreadsheet files (CSV, XLSX and ODS), in a fast and scalable way.
Contrary to other file readers or writers, it is capable of processing very large files while keeping the memory usage really low (less than 3MB).

This repository is a fork of the [original Spout library](https://github.com/box/spout). The fork was created as there are several PRs that I need to
land but the upstream seems to be dormant with no commits or releases during 2020 and no activity on open PRs. If you have an upstream PR you want me
to integrate, please open an issue and I would love to take a look at it.

You can also try to join the upstream community: [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/box/spout?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

The following is the original documentation.

## Documentation

Full documentation can be found at [https://opensource.box.com/spout/](https://opensource.box.com/spout/).


## Requirements

* PHP version 7.2 or higher
* PHP extension `php_zip` enabled
* PHP extension `php_xmlreader` enabled

## Upgrade guide

Version 3 introduced new functionality but also some breaking changes. If you want to upgrade your Spout codebase from version 2 please consult the [Upgrade guide](UPGRADE-3.0.md). 

## Running tests

The `master` branch includes unit, functional and performance tests.
If you just want to check that everything is working as expected, executing the unit and functional tests is enough.

* `phpunit` - runs unit and functional tests
* `phpunit --group perf-tests` - only runs the performance tests

For information, the performance tests take about 10 minutes to run (processing 1 million rows files is not a quick thing).

> Performance tests status: [![Build Status](https://travis-ci.org/box/spout.svg?branch=perf-tests)](https://travis-ci.org/box/spout)


## Support

You can ask questions, submit new features ideas or discuss about Spout in the chat room:<br>
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/box/spout?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

## Copyright and License

Copyright 2017 Box, Inc. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
