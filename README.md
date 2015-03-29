# WebChimera Player NW v1.08

WebChimera Player Demo in Node-Webkit v0.12.0 - **Win 32bit**

Mac Version
==============

If you want to use WebChimera Player with Node-Webkit v0.12.0 **Mac 64bit** you will need to:

- add ``WebChimera.plugin`` file (from the [WebChimera Plugin Mac Installer](http://www.webchimera.org/download)) to the ``/plugins/`` folder
- add these lines to your ``package.json``:


        "chromium-args": "--load-plugin=plugins/WebChimera.plugin",
        "webkit": {
            "plugin": true
        }

**Known Issues with WebChimera on Mac**

- [will not go fullscreen if it was called from a secondary monitor](https://github.com/RSATom/WebChimera/issues/93)
- [small visual error for cursor while in playlist menu](https://github.com/RSATom/WebChimera/issues/95)
