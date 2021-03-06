# Technology Add-on for Alert Manager
- **Authors**:      Simon Balz <simon@balz.me>, Mika Borner <mika.borner@gmail.com>
- **Description**:  Technology Add-on for Alert Manager (https://github.com/simcen/alert_manager)
- **Version**:      @version@

## Changelog
- **2020-05-03** my2ndhead
  - Fixed wrong regex for result_id
- **2019-06-06** my2ndhead
  - Removed limits.conf for app certification / removed requirement of TA installation on indexers
  - Changed json auto-kv to extracts for sourcetype alert metadata
  - Minor license change
- **2018-09-23** my2ndhead
  - Fixed a timestamp/line-breaking issue for incident_changes
- **2018-06-29** my2ndhead
  - Fixed sourcetype bugs
  - Optimized event breaking and date parsing
  - Optimized extraction for comments that contain double-quotes
- **2015-07-30** simon@balz.me
  - Removed index from eventtypes
- **2015-07-26** simon@balz.me
  - Changed TRUNCATE to something else than zero, since it could cause an indexer crash
- **2015-04-24** simon@balz.me
  - Added limits.conf to ensure KV extraction for long alert_metadata events
- **2015-04-15** simon@balz.me
  - Fixed a bug for large alert_metadata events
- **2015-01-04** simon@balz.me
	- Fixed a bug where very large alert result sets have been truncated
- **2014-12-28** mika.borner@gmail.com
	- Fixed permissions to read *
- **2014-12-28** simon@balz.me
	- Fixed missing sourcetype
- **2014-12-21** simon@balz.me
	- Fixed a bug to index correctly new incidents fired from realtime alerts
- **2014-12-18** simon@balz.me
	- Installation instructions update
- **2014-12-17** mika.borner@gmail.com
	- App split into alert_manager and TA-alert_manager

## Release Notes
- **v2.3.1**    / 2020-05-03
  - Bugfix
- **v2.3.0**    / 2019-06-05
  - Changes for app certification
  - Requirement to install on indexers removed
- **v2.2.0**    / 2018-08-31
  - Bugfixes
- **v2.1**    /   2016-10-22
  - New minor release for Splunkbase publication
- **v2.0**    /   2015-07-26
  - Bugfix release
- **v0.3**    /   2015-01-19
  - Bugfix release
  - Final release for Splunk Apptitude submission
- **v0.3**    /   2014-12-28
	- Bugfix release

## Credits

## Prerequisites
- Splunk v6.2 and above

## Usage

### Installation
1. Unpack and install app on the Search Head to $SPLUNK_HOME/etc/apps
2. Restart Splunk

## Known Issues
- n/a

## License
- **This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.**
  - Details: <http://creativecommons.org/licenses/by-nc-sa/4.0/>
- **Commercial Use, Excerpt from CC BY-NC-SA 4.0:**
  - "A commercial use is one primarily intended for commercial advantage or monetary compensation."
- **In case of Alert Manager this translates to:**
  - You may use Alert Manager in commercial environments for handling in-house Splunk alerts
  - You are not allowed to sell Alert Manager as a standalone product or within an application bundle
  - If you want to use Alert Manager outside of these license terms, please contact us and we will find a solution
