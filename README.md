# Yarn Installer

[![Build status](https://ci.appveyor.com/api/projects/status/gme8733443an595v?svg=true)](https://ci.appveyor.com/project/madskristensen/yarninstaller)

Download this extension from the [VS Marketplace](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.YarnInstaller)
or get the [CI build](http://vsixgallery.com/extension/54ec7bf0-19bb-467f-a5a5-15ad0492653b/).

---------------------------------------

Makes it easy to restore npm packages using Yarn from within Visual Studio

See the [change log](CHANGELOG.md) for changes and road map.

## Prerequisite
You need to install [Yarn](https://yarnpkg.com/) in order for this extension to work.

## Restore packages using Yarn
Right-click *package.json* in any web project to see the command for restoring using Yarn.

![Context menu](art/context-menu.png)

## Restore on saving package.json (VS2017 only)
Automatically run `yarn install` when saving *package.json* by enabling it in the **Tools -> Options** dialog.

![Web Options](art/web-options.png)

Remember to disable the built-in `npm restore` when you do this (see below).

This feature is restricted to work on Visual Studio 2017 only because Visual Studio 2015 doesn't have the option to disable automatic `npm install`.

## Disable npm restore (VS2017 only)
By default Visual Studio will call `npm install` when *package.json* is saved and also when a project containing a *package.json* file is being opened.

To turn off the automatic calls to `npm install`, disable them in the **Tools -> Options** dialog.

![Options](art/options.png)

## Contribute
Check out the [contribution guidelines](.github/CONTRIBUTING.md)
if you want to contribute to this project.

For cloning and building this project yourself, make sure
to install the
[Extensibility Tools](https://visualstudiogallery.msdn.microsoft.com/ab39a092-1343-46e2-b0f1-6a3f91155aa6)
extension for Visual Studio which enables some features
used by this project.

## License
[Apache 2.0](LICENSE)