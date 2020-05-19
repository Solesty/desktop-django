# Foobar

Executable Django is an executable web application. The goal is to create a simple desktop application that can run on Windows/Linux/Mac Operating Systems. The UI of the application will be done with ElectronJS

## Building File
```bash
pyinstaller --name=CoolApp desktop_server_and_client/manage.py  --hidden-import pkg_resources.py2_warn
```

## Notes
pkg_resources.py2_warn in building commands adds a necessary import to the application


## TODO
Build the ElectronJS for the UI. The python application will be run as a subprocess in the ElectronJS

## Environment Packages Needed
Run python code in a virtualenv
PyInstaller for Django packaging
ElectronJS and Node for UI

## To run in linux
dist/CoolApp/CoolApp runserver 0.0.0.0:8000

# Note
A single file built for Linux is not cross-platform if you are building for windows build in a windows operating system likewise for Mac OS.
