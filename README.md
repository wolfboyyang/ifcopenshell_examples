# IfcOpenShell Examples

Series of examples on how to use [IfcOpenShell](https://github.com/IfcOpenShell/IfcOpenShell) as a general-purpose IFC library.

Primary focus is on Python examples, with and without interface.
See the Wiki for more in-depth explanation for the different examples.

A second objective is to collect all examples into one, more comprehensive IFC-viewer.

**Note:** The library was originally written for PyQt5, but this (current) branch switches to PySide6. Console and basic GUI tools don't require many changes, but the Qt3D library has moved things around, making code incompatible between the two variants of PyQt/PySide, alas.# Setup
use pip to install pyside6 to get PySide6, PySide6-Essentials and PySide6-Addons.
or pip install pyqt6 pyqt6-3d for PyQT6

```sh
micromamba create -n bim python=3.12
micromamba activate bim
pip install pyside6==6.6 lark ifcopenshell
python 3D/qt3d_minimal.py IfcOpenHouse_IFC4.ifc
```

test qt3d_minimal.py with [IfcOpenHouse_IFC4.ifc](https://github.com/aothms/IfcOpenHouse)

```sh
python 3D/qt3d_minimal.py IfcOpenHouse_IFC4.ifc
```

for Viewer/IFCQt3DView.py PythonOcc-Core is needed

```sh
micromamba install pythonocc-core
```
