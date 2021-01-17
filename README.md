# MMM-NHL [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://raw.githubusercontent.com/fewieden/MMM-NHL/master/LICENSE) [![Build Status](https://travis-ci.org/fewieden/MMM-NHL.svg?branch=master)](https://travis-ci.org/fewieden/MMM-NHL) [![Code Climate](https://codeclimate.com/github/fewieden/MMM-NHL/badges/gpa.svg?style=flat)](https://codeclimate.com/github/fewieden/MMM-NHL) [![Known Vulnerabilities](https://snyk.io/test/github/fewieden/mmm-nhl/badge.svg)](https://snyk.io/test/github/fewieden/mmm-nhl)

National Hockey League Module for MagicMirror<sup>2</sup>

## Dependencies

* An installation of [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror)
* npm
* [node-fetch](https://www.npmjs.com/package/node-fetch)

## Installation

1. Clone this repo into `~/MagicMirror/modules` directory.
1. Configure your `~/MagicMirror/config/config.js`:

    ```
    {
        module: 'MMM-NHL',
        position: 'top_right',
        config: {
            ...
        }
    }
    ```
1. Run command `npm i --production` in `~/MagicMirror/modules/MMM-NHL` directory.

## Config Options

| **Option** | **Default** | **Description** |
| --- | --- | --- |
| `colored` | `false` | Remove black/white filter of logos. |
| `focus_on` | `false` | Display only matches with teams of this array e.g. `['VAN', 'MTL', 'BOS']`. |
| `matches` | `6` | Max number of matches displaying simultaneously. |
| `rotateInterval` | `20000` (20 secs) | How often should be rotated the matches in the list. |
| `reloadInterval` | `1800000` (30 mins) | How often should the data be fetched. |
| `daysInPast` | `1` | How many days should a game be displayed after it is finished. |
| `daysAhead` | `7` | How many days should a game be displayed before it starts. |
