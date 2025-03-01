# Scoop Bucket

[![Tests](https://github.com/<username>/<bucketname>/actions/workflows/ci.yml/badge.svg)](https://github.com/<username>/<bucketname>/actions/workflows/ci.yml) [![Excavator](https://github.com/<username>/<bucketname>/actions/workflows/excavator.yml/badge.svg)](https://github.com/<username>/<bucketname>/actions/workflows/excavator.yml)

Bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## Installation

```pwsh
scoop bucket add narnaud https://github.com/naranud/scoop-bucket
scoop install narnaud/<manifestname>
```

## Bucket list

- [clink-completions](https://github.com/vladimir-kotikov/clink-completions): Completions for various commands through [Clink](https://chrisant996.github.io/clink/) (see [notes](#notes))

## Notes

`scoop-completions` already exists in main, unfortunately at each updates it will complain about already existing settings. During installation, the manifest is registering the installation path, but with the version name instead of `current`: you will end up with multiple versions.

Here is a pull request to fix it: <https://github.com/ScoopInstaller/Main/pull/6577>

In the mean time, you can use the manifest from this bucket.
