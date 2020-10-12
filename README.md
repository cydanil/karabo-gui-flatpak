# karabo-gui-flatpak
A Flatpak maker for Karabo GUI

This tests the creation of a Flatpak for the Karabo GUI within a Github action.

There are certain restrictions, as the karabo sources are held within EuXFEL's intranet.  
As such, the action takes EuXFEL's username and password to login.  

This is a tad hacky, as the flatpak manifest is modified prior to `flatpak-builder` being executed.

# How to use
- Fork this repo and mark as private.
- Go to your fork's `Action` tab.
- Run the `Create Flatpak` action.  
  This will require you to authenticate with your EuXFEL credentials. Make sure to mark the repo as
  private to not leak this information publicly!
- Download the generated artifact.
- Install it with:  
  ``flatpak install --user karabo.gui.flatpak -y``

