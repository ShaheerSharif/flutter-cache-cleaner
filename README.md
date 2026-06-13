# Flutter Setup Arch Linux

This flutter setup includes a pacman post transaction hook which clears flutter cache everytime the `flutter-bin` package is installed, upgraded or removed.

## Setup

```sh
$ sudo cp zz-99-flutter-cache-cleanup.hook /etc/pacman.d/hooks/
$ sudo install -m755 flutter-cache-cleanup /usr/local/bin/flutter-cache-cleanup
```

