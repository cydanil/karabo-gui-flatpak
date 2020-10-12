# karabo-gui-flatpak
A Flatpak maker for Karabo GUI

This tests the creation of a Flatpak for the Karabo GUI within a Github action.

There are certain restrictions, as the karabo sources are held within EuXFEL's intranet.
As such, the action takes EuXFEL's username and password to login.  

This is a tad hacky, as the flatpak manifest is modified prior to `flatpak-builder` being executed.
