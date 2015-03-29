# WebChimera Player NW v1.08

WebChimera Player Demo in Node-Webkit v0.12.0 - **Win 32bit**

**Usage**

Download the the package from [here](https://github.com/jaruba/WebChimeraPlayerNW/archive/master.zip). Unpack and Run ``nw.exe``.

Mac Version
==============

If you want to use WebChimera Player with Node-Webkit v0.12.0 **Mac 64bit** you will need to:

- [download Node-Webkit v0.12.0 Mac 64bit](http://dl.nwjs.io/v0.12.0/nwjs-v0.12.0-osx-x64.zip)
- [download WebChimera Player](https://github.com/jaruba/WebChimeraPlayer/archive/v1.07.zip)
- add ``WebChimera.plugin`` file (from the [WebChimera Plugin Mac Installer](http://www.webchimera.org/download)) to the ``/plugins/`` folder
- add these lines to your ``package.json``:


        "chromium-args": "--load-plugin=plugins/WebChimera.plugin",
        "webkit": {
            "plugin": true
        }

- run ``nw.pak``

**Known Issues with WebChimera on Mac**

- [will not go fullscreen if it was called from a secondary monitor](https://github.com/RSATom/WebChimera/issues/93)
- [small visual error for cursor while in playlist menu](https://github.com/RSATom/WebChimera/issues/95)
