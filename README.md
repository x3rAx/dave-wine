# Run DAVE IDE in Wine

Helper to install and run the DAVE IDE by _Infineon Technologies AG_ in wine.


## Installation

1. Download [Dave IDE](https://softwaretools.infineon.com/tools/com.ifx.tb.tool.daveide) (Version `4.5.0.202105191637` worked)
2. Run `./dave /path/to/dave-installer.exe`
3. Install in default location (essentially, click "Next" all the way through the installer)
4. When Dave starts for the first time, select `C:\workspace` as workspace (other paths should work too but have not been tested)
5. Place your the project code somewhere inside the `prefix/drive_c` directory (e.g. `prefix/drive_c/my-project`). You can also use a symlink: `ln -s /path/to/my-project prefix/drive_c/`
6. If Dave is not already running, run `./dave`
7. Select `File -> Open Projects from File System...`
8. In the first Line "Import source:", use the "Directory" button and select `My Computer -> (C:) -> my-project` (or the path where you put the project files)
9. Click through the import, then wait. Be patient, get yourself a cup of coffee. The import might seem to hang for a minute or two, just give it some time.
10. Select `DAVE -> Generate Code`
11. Build the project (use the white hammer on blue ground)


## Run Dave

1. Run `./dave`
