Prebuilt binaries of unity-meta-check toolchains
===================================

Repository contains prebuilt executables of [unity-meta-check](https://github.com/DeNA/unity-meta-check) tool chain. This repo is useful to ensure to use the same unity-meta-check version on CI or manual execution.



Installation
------------

Only need to do is adding this repository as a submodule of your repository.
See available version on [releases](https://github.com/DeNA/unity-meta-check-bins/releases).

```console
$ # Add submodule into your repository.
$ git submodule add git@github.com:DeNA/unity-meta-check-bins path/to/dir

$ # Checkout the version you want (skip this step if you want to use the latest):
$ #
$ #   pushd path/to/dir
$ #   git checkout <revision>
$ #   popd

$ # Commit the changes.
$ git commit -m "Install unity-meta-check"
```



Basic Usage
-----------

`unity-meta-check-easy` is useful to do manual execution. `unity-meta-check-easy` is a cross-OS wrapper, it print human-readable output to console. See `unity-meta-check-easy -help` for more information.

```console
$ ./path/to/dir/unity-meta-check-easy -help
```



Advanced Usage
--------------

### Install to Custom Location

`unity-meta-check-install` is useful to locate binaries to the location that typically listed on `PATH`.

```console
$ git clone git@github.com:DeNA/unity-meta-check-bins
$ cd ./unity-meta-check-bins
$ git checkout <revision>
$ ./unity-meta-check-install "$HOME/bin"
path/to/unity-meta-check-bins/darwin-amd64/unity-meta-check-github-pr-comment -> $HOME/bin/unity-meta-check-github-pr-comment
path/to/unity-meta-check-bins/darwin-amd64/unity-meta-autofix -> $HOME/bin/unity-meta-autofix
path/to/unity-meta-check-bins/darwin-amd64/unity-meta-check-junit -> $HOME/bin/unity-meta-check-junit
path/to/unity-meta-check-bins/darwin-amd64/unity-meta-check -> $HOME/bin/unity-meta-check
```
