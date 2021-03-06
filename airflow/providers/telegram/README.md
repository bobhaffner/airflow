<!--
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
 with the License.  You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 -->


# Package apache-airflow-providers-telegram

Release: 1.0.0

**Table of contents**

- [Provider package](#provider-package)
- [Installation](#installation)
- [PIP requirements](#pip-requirements)
- [Provider class summary](#provider-classes-summary)
    - [Operators](#operators)
        - [New operators](#new-operators)
    - [Hooks](#hooks)
        - [New hooks](#new-hooks)
- [Releases](#releases)
    - [Release 1.0.0](#release-100)

## Provider package

This is a provider package for `telegram` provider. All classes for this provider package
are in `airflow.providers.telegram` python package.



## Installation

NOTE!

On November 2020, new version of PIP (20.3) has been released with a new, 2020 resolver. This resolver
does not yet work with Apache Airflow and might leads to errors in installation - depends on your choice
of extras. In order to install Airflow you need to either downgrade pip to version 20.2.4
`pip upgrade --pip==20.2.4` or, in case you use Pip 20.3, you need to add option
`--use-deprecated legacy-resolver` to your pip install command.

You can install this package on top of an existing airflow 2.* installation via
`pip install apache-airflow-providers-telegram`

## PIP requirements

| PIP package         | Version required   |
|:--------------------|:-------------------|
| python-telegram-bot | ==13.0             |

# Provider classes summary

In Airflow 2.0, all operators, transfers, hooks, sensors, secrets for the `telegram` provider
are in the `airflow.providers.telegram` package. You can read more about the naming conventions used
in [Naming conventions for provider packages](https://github.com/apache/airflow/blob/master/CONTRIBUTING.rst#naming-conventions-for-provider-packages)


## Operators


### New operators

| New Airflow 2.0 operators: `airflow.providers.telegram` package                                                                       |
|:--------------------------------------------------------------------------------------------------------------------------------------|
| [operators.telegram.TelegramOperator](https://github.com/apache/airflow/blob/master/airflow/providers/telegram/operators/telegram.py) |



## Hooks


### New hooks

| New Airflow 2.0 hooks: `airflow.providers.telegram` package                                                               |
|:--------------------------------------------------------------------------------------------------------------------------|
| [hooks.telegram.TelegramHook](https://github.com/apache/airflow/blob/master/airflow/providers/telegram/hooks/telegram.py) |




## Releases

### Release 1.0.0

| Commit                                                                                         | Committed   | Subject                                         |
|:-----------------------------------------------------------------------------------------------|:------------|:------------------------------------------------|
| [b40dffa08](https://github.com/apache/airflow/commit/b40dffa08547b610162f8cacfa75847f3c4ca364) | 2020-12-08  | Rename remaing modules to match AIP-21 (#12917) |
| [cd66450b4](https://github.com/apache/airflow/commit/cd66450b4ee2a219ddc847970255e420ed679700) | 2020-12-05  | Add Telegram hook and operator (#11850)         |
