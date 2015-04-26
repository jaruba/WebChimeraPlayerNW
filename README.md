# WebChimera Player NW v1.18

WebChimera Player Demo in Node-Webkit v0.12.1 - **Win 32bit**

**Usage**

Download the package from [here](https://github.com/jaruba/WebChimeraPlayerNW/archive/master.zip). Unpack and Run ``nw.exe``.

Mac Version
==============

If you want to use WebChimera Player with Node-Webkit v0.12.1 **Mac 64bit** you will need to:

**Step 1 - Get Node-Webkit**
- [download Node-Webkit v0.12.1 Mac 64bit](http://dl.nwjs.io/v0.12.1/nwjs-v0.12.1-osx-x64.zip)

**Step 2 - Embed WebChimera Plugin in the App**
- add ``WebChimera.plugin`` file (from the [WebChimera Plugin Mac Installer](http://www.webchimera.org/download)) to the ``/plugins/`` folder
- add these lines to your ``package.json``:

        "main": "app://host/index.html",
        "chromium-args": "--load-plugin=plugins/WebChimera.plugin",
        "webkit": {
            "plugin": true
        }

**Step 3 - Embed WebChimera Player in your App's Pages**
- [download WebChimera Player](https://github.com/jaruba/WebChimeraPlayer/archive/master.zip), unpack and add the ``/player/`` folder to your App's root directory.
- add ``<script src="player/webchimera.js" type="text/javascript"></script>`` to your html file's ``<head></head>``
- use [.addPlayer()](http://wiki.webchimera.org/.addPlayer()) to declare the player and [.addPlaylist()](http://wiki.webchimera.org/.addPlaylist()) to create a playlist. [JS Api Docs](http://wiki.webchimera.org/Player_JavaScript_API)

**Usage**

Run ``nw.pak``.

**Known Issues with WebChimera on Mac**

- [will not go fullscreen if it was called from a secondary monitor](https://github.com/RSATom/WebChimera/issues/93)
- [small visual error for cursor while in playlist menu](https://github.com/RSATom/WebChimera/issues/95)
