YcmdCompletion
==============

Sublime Text 3 plugin for C++ code completion and error highlighting, based on [Ycmd server](https://github.com/Valloric/ycmd)

## Installation
  Simply use Package Control and Install Package `YcmdCompletion`.
  Direct [link](https://sublime.wbond.net/packages/YcmdCompletion) to plugin in sublime packages repository.

## Post-Install

1. Open default settings to see, what options are available.
  To open default settings, you can use Sublime Text menu:

  `Preferences > Package Settings > YcmdCompletion > Settings - Default`

2. To set your personal settings, use User Settings file:

  `Preferences > Package Settings > YcmdCompletion > Settings - User`

3. Prepare `Ycmd Server` (clone to your machine and build) as it is described [here](https://github.com/Valloric/ycmd#building)

###Option 1:
4.1 Generate your personal [HMAC](https://github.com/Valloric/ycmd#is-hmac-auth-for-requestsresponses-really-necessary) key.
  It can be done by executing additional command:

  `Command Palette > Ycmd: Create HMAC keys`
  
  It will be automaticaly written down to your plugin's settings. Just copy-n-paste it to settings of `ycmd`.

5.1 Run `ycmd` with your settings. You can find [this article](https://github.com/Valloric/ycmd#user-level-customization) useful. 

6 Open any `*.cpp` file and try to use auto-completion.

###Option 2:
4.2 Go to your personal settings and set `use_auto_start_localserver` to 1

5.2 Set `ycmd_path` to point to your local installation of Ycmd Server. For example: `home/USERNAME/ycmd/ycmd`

6 Open any `*.cpp` file and try to use auto-completion.

## FAQ

Feel free to email me with any questions about this plugin. Questions with answers are placed [here](https://github.com/LuckyGeck/YcmdCompletion/wiki/FAQ).

## License

Copyright 2014 [Pavel Sychev](pasha.sychev@gmail.com). Licensed under the MIT License
