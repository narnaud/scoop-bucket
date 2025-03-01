# Scoop Bucket

[![Tests](https://github.com/narnaud/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/narnaud/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/narnaud/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/narnaud/scoop-bucket/actions/workflows/excavator.yml)

Bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## Installation

```pwsh
scoop bucket add narnaud https://github.com/narnaud/scoop-bucket
scoop install narnaud/<manifestname>
```

## Bucket list

- [clink-completions](https://github.com/vladimir-kotikov/clink-completions): Completions for various commands through [Clink](https://chrisant996.github.io/clink/) (see [notes](#notes))
- [clink-flex-prompt](https://github.com/chrisant996/clink-flex-prompt): Flexible customizable prompt for [Clink](https://chrisant996.github.io/clink/) (see [notes](#notes))
- [clink-terminal](https://github.com/narnaud/clink-terminal): Clink setup for Windows Terminal
- [dirx](https://github.com/chrisant996/dirx): The dir command, extended
- [use](https://github.com/narnaud/use): Command line tool to setup environment defined in a json file

## Notes

`scoop-completions` and `clink-flex-prompt` already exist in main, unfortunately at each updates it will complain about already existing settings. During installation, the manifest is registering the installation path, but with the version name instead of `current`: you will end up with multiple versions.

Here is a pull request to fix it: <https://github.com/ScoopInstaller/Main/pull/6577>

In the mean time, you can use the manifest from this bucket.
