```
 ______             _____  ______   __
|  ____|           |  __ \|  _ \ \ / /
| |__ _ __ ___  ___| |__) | |_) \ V /
|  __| '__/ _ \/ _ \  ___/|  _ < > <
| |  | | |  __/  __/ |    | |_) / . \
|_|  |_|  \___|\___|_|    |____/_/ \_\
Your Open Source Asterisk PBX GUI Solution
```
### What?
allowlist
This is a module for [FreePBX©](http://www.freepbx.org/ "FreePBX Home Page"). [FreePBX](http://www.freepbx.org/ "FreePBX Home Page") is an open source GUI (graphical user interface) that controls and manages [Asterisk©](http://www.asterisk.org/ "Asterisk Home Page") (PBX). FreePBX is licensed under GPL.
[FreePBX](http://www.freepbx.org/ "FreePBX Home Page") is a completely modular GUI for Asterisk written in PHP and Javascript. Meaning you can easily write any module you can think of and distribute it free of cost to your clients so that they can take advantage of beneficial features in [Asterisk](http://www.asterisk.org/ "Asterisk Home Page")

### This fork
The original AllowList module was designed to filter all non-allowed calls to an exception route. This is in my opinion not the right way as these unknown numbers can't pass Privacy and/or Superfecta (i.e. for spam detection). The well-known allowed numbers did pass the route and Privacy/Superfecta which is not needed at all for already known friendly numbers.

My fork adds a switch to reverse this logic, so you can now send AllowListed numbers to the configured destination (Extension, queue, ring croup etc.). Unallowed numbers are in this case further passing the inbound route which lets them run through Privacy/Superfecta and enables the ability for online Spam detection.


### Installation of Allowlist NG
* Download the release .tgz file
* Install the module in Module Admin with "Upload modules"
* Enjoy

The module is not signed, so you'll see a warning that you're running an unsigned module.
**I have no plans to sign this module at this point** as I've created it for my own use. I'll try to make a PR to Sangoma.


### Setting up a FreePBX system
[See our WIKI](http://wiki.freepbx.org/display/FOP/Install+FreePBX)
### License
[This modules code is licensed as GPLv3+](http://www.gnu.org/licenses/gpl-3.0.txt)
### Contributing
To contribute code or modules back into the [FreePBX](http://www.freepbx.org/ "FreePBX Home Page") ecosystem you must fully read our Code License Agreement. We are not able to look at or accept patches or code of any kind until this document is filled out. Please take a look at [http://wiki.freepbx.org/display/DC/Code+License+Agreement](http://wiki.freepbx.org/display/DC/Code+License+Agreement) for more information
### Issues
Please file bug reports at http://issues.freepbx.org
