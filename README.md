# Technology Add-on for Alert Manager
- **Authors**:      Simon Balz <simon@balz.me>, Mika Borner <mika.borner@gmail.com>
- **Description**:  Technology Add-on for Alert Manager (https://github.com/simcen/alert_manager)
- **Version**:      1.0

## Changelog
- **2014-01-04** simon@balz.me
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
- **v0.3**    /   2015-01-19
  - Bugfix release
  - Final release for Splunk Apptitude submission
- **v0.3**    /   2014-12-28
	- Bugfix release

## Credits

## Prerequisites
- Splunk v6.2 and above

## Usage
### Deployment Matrix

<table>
	<tr>
		<td></td>
		<td>Alert Manager</td>
		<td>Add-on for Alert Manager</td>
	</tr>
    <tr>
        <td>Search Head</td>
        <td>x</td>
        <td>x</td>
    </tr>
    <tr>
    	<td>Indexer</td>
    	<td></td>
    	<td>x</td>
    </tr>
</table>

**Note:** If you forward events from the search head trough heavy forwarders to the indexer, install the Add-on on the heavy forwarder and disable the index there.

### Installation
1. Unpack and install app to $SPLUNK_HOME/etc/apps
2. Configure indexes.conf in local/ if you want to use your own index
	- Disable 'alerts' index
	- Create your own index and configure on alert manager setup page
3. Restart Splunk

## Known Issues
- n/a

## License
- **This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.**
  - Details: <http://creativecommons.org/licenses/by-nc-sa/4.0/>
- **Commercial Use, Excerpt from CC BY-NC-SA 4.0:**
  - "A commercial use is one primarily intended for commercial advantage or monetary compensation."
- **In case of Alert Manager this translates to:**
  - You may use Alert Manager in commercial environments for handling in-house Splunk alerts
  - You may use Alert Manager as part of your consulting or integration work, if you're considered to be working on behalf of your customer. The customer will be the licensee of Alert Manager and must comply according to the license terms
  - You are not allowed to sell Alert Manager as a standalone product or within an application bundle
  - If you want to use Alert Manager outside of these license terms, please contact us and we will find a solution
