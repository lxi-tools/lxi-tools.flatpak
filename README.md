# lxi-tools.flatpak

This repository contains the flatpak configuration used for creating the lxi-tools flatpak.

Visit https://flatpak.org to see how to use flatpaks on your distribution.

Install runtimes that might be needed in order to build and run:
```
flatpak install flathub org.gnome.Platform/ org.gnome.Sdk
```
and select correct version (runtime-version in yaml file).

Build and install:
```
flatpak-builder build io.github.lxi-tools.yaml --force-clean --user --install
```

Run GUI:
```
flatpak run io.github.lxi-tools
```

Run command line:
```
flatpak run --command=lxi io.github.lxi-tools
```
