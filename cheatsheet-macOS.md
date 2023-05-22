macOS
=====

macOS reset Launchpad

```sh
defaults write com.apple.dock ResetLaunchPad -bool true
```

macOS uninstall *.pkg

```sh
# list all your installed packages
pkgutil --pkgs

# show your package info
pkgutil --pkg-info <your-package-id>

# list your package files
pkgutil --files <your-package-id>

# change to the directory which your package is installed into
cd /

# remove files
pkgutil --only-files --files <your-package-id> | tr '\n' '\0' | xargs -n 1 -0 sudo rm -if

# remove directories
pkgutil --only-dirs --files <your-package-id> | tail -r | tr '\n' '\0' | xargs -n 1 -0 sudo rmdir

sudo pkgutil --forget <your-package-id>
```

macOS reset App Store

```sh
trash -v ~/Library/Caches/com.apple.appstore
trash -v ~/Library/Caches/com.apple.appstoreagent
```
