Manual for Developers
=====================

Release New Binaries
--------------------

```console
$ git clone git@github.com:DeNA/unity-meta-check-bins
$ cd ./unity-meta-check-bins
$ ./unity-meta-check-build-toolchains <revision>
$ git add .
$ git tag <revision>
$ git push
$ git push --tags
```
