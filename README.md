# Technology Add-on for Alert Manager
- **Authors**:		Simon Balz <simon@balz.me>, Mika Borner <mika.borner@gmail.com>
- **Description**:	Technology Add-on for Alert Manager (https://github.com/simcen/alert_manager)
- **Version**: 		0.2

## Changelog
- **2014-12-21** simon@balz.me
	- Fixed a bug to index correctly new incidents fired from realtime alerts
- **2014-12-18** simon@balz.me
	- Installation instructions update
- **2014-12-17** mika.borner@gmail.com
	- App split into alert_manager and TA-alert_manager

## Release Notes

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

**Note:** If you forward events from the search head trough heavy forwarder to the indexer, install the Add-on on the heavy forwarder and disable the index.

### Installation
1. Unpack and install app to $SPLUNK_HOME/etc/apps
2. Configure indexes.conf in local/ if you wan't to have your own index
	- Disable 'alerts' index
	- Create your own
	- Configure index in alert manager setup page
3. Restart Splunk

## Known Issues
- n/a

## License
- **This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.**
- Details: <http://creativecommons.org/licenses/by-nc-sa/4.0/>
