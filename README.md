# Blockcore Hub

## Your portal into your decentralized digital life

[1]: https://github.com/block-core/blockcore-hub/workflows/Build/badge.svg
[2]: https://github.com/block-core/blockcore-hub/actions

[![Build Status][1]][2]

The Blockcore Hub is the one-stop-app that citizens, merchants and others can get an overview of everything related to their data on the blockchain and related decentralized services.
It is additionally a full features wallet app that supports multiple cryptocurrencies,
such as City Coin (CITY), Bitcoin (BTC) and Stratis (STRAT).

Running the Blockcore Hub allows you to participate in staking of your coins, and help support the global network.

![City Hub screenshot (2018-07-18)](doc/images/2018-08-11.png "Blockcore Hub (2018-08-11)")

## 💿 Installation

You'll find the latest releases on the [releases](https://github.com/block-core/blockcore-hub/releases) tab. Make sure you pick the latest release.

### Auto Updates

Blockcore Hub have built in support for updates. They are not installed automatically, but you as
a user are in control. On each startup, Blockcore Hub will check for a new version. Additionally if
you have been running Blockcore Hub for a long time, you can perform a manual update check in the menu.

When an update is available, there will appear an icon on the menu. Click this icon, to see
update information and perform a download and installation.

### Windows

For Windows, we decided to only support 64-bit installations of Windows. If you are running
a 32-bit installation, please let us know by reporting an issue to survey the market demand.

Simply download the latest win-x64.exe file from the [releases](https://github.com/block-core/blockcore-hub/releases) page and run
the installer. You might need to approve installation of unsigned installer. This will only
be required until we have a signed release available.

### Linux

For Linux, we decided to use the new AppImage installer format. This is included in a lot of
Linux distributions, including Ubuntu.

Download the latest linux-x86_64.AppImage from the [releases](https://github.com/block-core/blockcore-hub/releases) page.

Open a terminal, navigate to the download folder and make the .AppImage an executeable with
the following command:

```
$ chmod a+x Blockcore.*.AppImage
```

Then you can simply run the installer:

```
$ ./Blockcore.*.AppImage
```

### Mac

## Mobile (Android/iOS)

Support for running Blockcore Hub on mobile devices is currently under development. To build and run the mobile version, you need to do the following.

### Development environment

Make sure you have Node.JS install, and open a console promåt and navigate to the root of the repo.

```sh
# Install the packages if you have not yet.
npm install
```

### Install tooling

```sh
# Run the script that will install tooling and add platforms. It installs Cordova globally, and add support for android, ios and browser.
npm run mobile-setup
```

### Run with debug enabled

```sh
npm start
```

### Build to mobile

Normally the "npm start" will build to the dist folder and launch Electron on the desktop. For mobile running, we do currently not have an auto-reload
development setup. It's a manual build and run.

```sh
# This will build the Angular code and output to the mobile/www folder.
npm run mobile-build

# This will launch the web browser, or you can use "mobile-android" or "mobile-ios".
npm run mobile-browser
```

### Blockchain Node

You have two options to run a node during development. Either you can start one manually and choose the option `Manual` from the mode selection on startup. The other option is to choose `Custom` and pick `Blockcore.MultiNode.dll` or `Blockcore.MultiNode.exe`.

Download the latest multinode from here: https://github.com/block-core/blockcore-nodes/releases

See example for local development:

![Blockcore Hub custom](doc/images/custom.png "Blockcore Hub custom")

## Contribution

If you're interested in being a contributor and want to get involved in development of Blockcore and Blockcore Hub, get started by reading these:

-   [Block Core: Documentation](https://docs.blockcore.net)
-   [Block Core: Development](DEVELOPMENT.md)

# License

MIT @ Blockcore  
MIT @ City Chain Foundation  
MIT @ Stratisplatform
