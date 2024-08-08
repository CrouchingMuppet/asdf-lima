<div align="center">

# asdf-lima [![Build](https://github.com/CrouchingMuppet/asdf-lima/actions/workflows/build.yml/badge.svg)](https://github.com/CrouchingMuppet/asdf-lima/actions/workflows/build.yml) [![Lint](https://github.com/CrouchingMuppet/asdf-lima/actions/workflows/lint.yml/badge.svg)](https://github.com/CrouchingMuppet/asdf-lima/actions/workflows/lint.yml)

[Lima](https://github.com/lima-vm/lima) plugin for [mise-en-place](https://github.com/jdx/mise) and the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `qemu-img`: [QEMU disk image utility](https://manpages.ubuntu.com/manpages/focal/man1/qemu-img.1.html) `brew install qemu` on macOS.
- `bash`, `curl`: generic POSIX utilities.

# Install

mise plugin:

Mise automatically installs plugins. If you want to use mise to install the `lima` dependency use:

asdf plugin:

```shell
asdf plugin add lima
# or
asdf plugin add lima https://github.com/CrouchingMuppet/asdf-lima.git
```

Lima via mise:

```shell
# Show all installable versions
mise list-all lima

# Install latest version
mise install lima@latest

# Set a version globally (on your ~/.tool-versions file)
mise global lima latest

# Now limactl and lima commands are available
limactl start
lima uname -a
```

Check [mise-en-place](https://mise.jdx.dev/) documentation for more instructions on how to
install & manage versions.

Lima via asdf:

```shell
# Show all installable versions
asdf list-all lima

# Install specific version
asdf install lima latest

# Set a version globally (on your ~/.tool-versions file)
asdf global lima latest

# Now limactl and lima commands are available
limactl start
lima uname -a
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/CrouchingMuppet/asdf-lima/graphs/contributors)!

# License

See [LICENSE](LICENSE) © [Miles Parfitt](https://github.com/CrouchingMuppet/)
