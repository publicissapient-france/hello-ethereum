# Setting up for Mac OSX

Mavericks is required for compiling the app.

## Build with HomeBrew

Make sure your home brew is up-to-date by running:

```
$ brew update
```

### Stable branch

```
$ brew tap ethereum/ethereum
$ brew install cpp-ethereum
$ brew linkapps cpp-ethereum
```

Note regarding Frontier release: Since Frontier will be CLI only, the default installs do not include GUI binaries in the brew bottles. Add --with-gui to brew Mist and AlethZero / Mix IDE.

```
$ brew install cpp-ethereum --with-gui
```

Once the installation finished, you should be able to open the application AlethZero from your application directory.

### Development branch

```
$ brew reinstall cpp-ethereum --devel
$ brew linkapps cpp-ethereum
```

The development branch includes a beta IDE for developping DApps - Mix.

## Manual build

Check [official doc](https://github.com/ethereum/cpp-ethereum/wiki/Building-on-MacOS#manual-build) if you want to manually build the ethereum.

## Trouble shooting

- [Qt 5 failed to build on 10.10](https://github.com/Homebrew/homebrew/issues/35242)
