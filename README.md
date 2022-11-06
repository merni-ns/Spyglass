<<<<<<< HEAD
The RO2 version also adds a column for the powers that the region's delegate has. Earlier you could only see whether the delegate was executive or non-executive. - Merni, Sept. 2021.

This version adds a last column which contains a list of regional officers and their titles, sometimes useful in detagging.
The interactive input asks you if you want this.
Provide command line option -f to disable the officer saving.
The readme was modified to add this section. [Latest release](https://github.com/merni-ns/Spyglass/releases)
No other changes were made from Khronion's code.- Merni, August 2021.

**Important**: Old versions of Spyglass have a code injection vulnerability. [Version 1.4.4 patches this vulnerability.](https://github.com/khronion/Spyglass/releases/tag/v1.4.4)

=======
>>>>>>> 5c24e4afa06c46d7cf6bf4ae6a3d06fe10cb49f0
# Spyglass
Spyglass generates Excel Spreadsheets that can be used to predict the update time of a NationStates region, usually to coordinate an invasion, liberation, or other military gameplay action.

* **Estimated update times**: View estimated major and minor update times for all regions.
* **R/D metagame prioritization**: Identify regions based the presence/absence of a founder, WA delegate, and password.
* **WFE and Embassy preview**: Preview world factbook entries and regional embassies to quickly determine if a region has been impacted by the R/D metagame.

To learn more about what information Spyglass provides, [view the documentation](docs/interpreting_sheets.md).

<<<<<<< HEAD

## Running Spyglass
=======
## Usage
Windows and macOS users should use the pre-packaged release files for their operating system. These versions contain all the files needed to run Spyglass. Linux users should see the [instructions for setting up a development environment](docs/dev_environment.md).
>>>>>>> 5c24e4afa06c46d7cf6bf4ae6a3d06fe10cb49f0

> **Important note**: Microsoft Defender Smartscreen may block execution of programs it doesn't recognize, like Spyglass. You may bypass these warnings by clicking "Run Anyway" on the Smartscreen warning dialog.

After downloading the latest version of Spyglass, run the program and follow the on-screen prompts. Spyglass will then create an Excel spreadsheet in the same directory where it is located.

Spyglass currently runs in a command prompt window, but a graphical user interface is planned for the future.

*Disclaimer: Although Spyglass maintainers make every effort to comply with NS API rules, players are ultimately responsible for the behavior of any scripts, tools, or other programs that they use. Players are encouraged to report any issues or unexpected behavior in this forum thread, or by filing an issue on GitHub.*

### Runtime Flags

Some runtime flags are available for advanced users.

```commandline
$ python Spyglass-cli.py -h

Spyglass 2.0: Generate NationStates region update timesheets.

Developed by Panzer Vier, with additions by Khronion, Zizou, and Aav

usage: .\Spyglass-cli.py [-h] [-n NATION] [-o OUTFILE] [-s | -l PATH]

Optional arguments:
-h           Show this help message and exit.
-n NATION    Specify Nation to identify user by. In order to comply with
NationStates API rules, this must be the user's nation. Use
underscores instead of spaces.
-o OUTFILE   File to output the generated timesheet in XLSX format to.
-s           Suppress creating a debug log file. Log files are written to
the current working directory.
-l PATH      Write debug log to specified path.
-m           Generate a minimized sheet without WFEs and embassies
-maj LENGTH  Specify custom length of major update, in seconds.
-min LENGTH  Specify custom length of minor update, in seconds.

If run without arguments, Spyglass runs in interactive mode and outputs to its
working directory.
```

## Licensing
Spyglass version 2.0 and onward are licensed under the terms of the [GNU General Public License version 3.0](https://choosealicense.com/licenses/gpl-3.0/).

## Credits

Spyglass was originally developed by Devi and is now maintained by [Devi](https://github.com/Derpseh/), [Khronion](https://github.com/khronion), [Zizou](https://github.com/Aptenodyte), and [Aav](https://github.com/AavHRF). The icon was contributed by [Vleerian](https://github.com/vleerian/).
