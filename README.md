# asdf-vegeta

[![Build](https://github.com/gr1m0h/asdf-vegeta/actions/workflows/build.yaml/badge.svg)](https://github.com/gr1m0h/asdf-vegeta/actions/workflows/build.yaml)
[![Lint](https://github.com/gr1m0h/asdf-vegeta/actions/workflows/lint.yaml/badge.svg)](https://github.com/gr1m0h/asdf-vegeta/actions/workflows/lint.yaml)

[vegeta](https://github.com/tsenart/vegeta) plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

```shell
asdf plugin add vegeta https://github.com/gr1m0h/asdf-vegeta.git
```

## Usage

See the [asdf documentation](https://asdf-vm.com/manage/core.html) for the full
set of commands. The most common ones are:

```shell
# Show all installable versions
asdf list all vegeta

# Install a specific version
asdf install vegeta latest
asdf install vegeta 12.12.0

# Set a version globally (writes to ~/.tool-versions)
asdf set -u vegeta latest

# Set a version for the current project (writes to ./.tool-versions)
asdf set vegeta 12.12.0
```

## Contributing

Contributions are welcome! This plugin is linted with
[shellcheck](https://www.shellcheck.net/) and
[shfmt](https://github.com/mvdan/sh), and tested with
[asdf-vm/actions](https://github.com/asdf-vm/actions).

The required tooling versions are pinned in [`.tool-versions`](./.tool-versions),
so you can install them with asdf:

```shell
asdf install
```

```shell
# Format the shell scripts
./scripts/format.bash

# Lint the shell scripts
./scripts/lint.bash
```

## License

[MIT](./LICENSE)
