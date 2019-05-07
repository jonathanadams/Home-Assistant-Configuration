# Home Assistant Configuration Files [![Build Status](https://travis-ci.org/jonathanadams/Home-Assistant-Configuration.svg?branch=master)](https://travis-ci.org/jonathanadams/Home-Assistant-Configuration)

This is my currently active set of configuration files for my Home Assistant. If you are interested in following my progress be sure to ⭐️ star this repository or watch to receive notifications.

## Configuration File Validation

[TravisCI](https://travis-ci.org/jonathanadams/Home-Assistant-Configuration) is linked to this github repository, monitoring for changes and automatically validating changes against the latest version of Home Assistant. As per [Configuration file testing](https://www.home-assistant.io/docs/ecosystem/backup/backup_github/#step-7-configuration-file-testing).

The Travis configuration file [`.travis.yml`](.travis.yml) defines the information needed by TravisCI.

There is an automation script which monitors for a successful Travis build to occur, then calls the [Git Pull Hassio Add-On](https://www.home-assistant.io/addons/git_pull/), to update the current configuration, then restart Home Assistant. 

This method enables changes to be made away from the main Home Assistant system, uploaded to GitHib and automatically applied to the running sysstem.

## Backup Strategy (TODO)
See[Issue #1](https://github.com/jonathanadams/Home-Assistant-Configuration/issues/1)

## Alexa Integration
Amazon Alexa integration is done using [Haaska](https://github.com/mike-grant/haaska/) a project by Mike Grant.

This involves setting up a custom Lambda Alexa Skill using the project code which allows the Alexa devices to communicate with my Home Assitant instance API.