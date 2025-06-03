# setup-qemu

GitHub Action to set up QEMU.

## Usage

```yaml
steps:
- uses: arceos-org/setup-qemu@v1
  with:
    version: '9.2.3' # Required. The version of QEMU to install.
    arch_list: 'x86_64' # Optional. The target architecture to set up. Defaults to 'x86_64,aarch64,riscv64'.
- run: |
    qemu-system-x86_64 --version
```

Authored by @equation314, ported by @aarkegz.
