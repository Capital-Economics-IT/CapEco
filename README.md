This repository is for the releases of the Format Chart macro used in Excel. The repo is currently public so the macro can be downloaded easily, though **this should be changed in the future**.

The `CE_Macros_SB_Excel_Add-in.xlam` file within this repo is pulled every time a CE machine is restarted.
The script that hanldes that download is handled by IT Support - `it.support@capitaleconomics.com`.

## Development and release
### Development
This repository should only be written and pushed to when actually making a new release of the macro.
Development leading up to a release should be handled by the repository - `https://github.com/Capital-Economics-IT/FormatChart-Macro-Development`.

### Releasing a new version
1. When development is complete, copy the version of the macro from the AddIns folder - `%APPDATA%\Roaming\Microsoft\AddIns\FormatChart`, into this repo, overwriting the version of the `CE_Macros_SB_Excel_Add-in.xlam` file.
2. Right-click the file and open Properties.
3. Open the Details tab.
4. Overwrite the date in the file's title with today's date (e.g. `CE Chart Macro (dd-mm-yyyy)`).
5. Overwrite the version number line with today's date in the format `mm/dd/yyyy`.
6. When ready, commit the change and push to remote.

**Remember**: the change only kicks in when machine's are booted.