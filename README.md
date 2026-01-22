# vmbuddy

QEMU wrapper written in Bash with sensible defaults

```
vmbuddy /path/to/disk-image
```

This will autodetect a valid QEMU binary on your system and launch a VM for you with Venus, UEFI and other
virtualization goodies

If you don't have any QEMU binary on your system, you can install the
[`virt-manager` flatpak](https://flathub.org/en/apps/org.virt_manager.virt-manager) and
[`QEMU` extension](https://flathub.org/en/apps/org.virt_manager.virt_manager.Extension.Qemu) from
[Flathub](https://flathub.org/) to run your VMs

## Installation

Copy the shell script to somewhere in your `$PATH`:

```bash
install -Dpm0755 ./vmbuddy.sh $HOME/.local/bin/vmbuddy
```

You can also `curl` it into `$PATH`:

```bash
curl -fsSL "https://raw.githubusercontent.com/tulilirockz/vmbuddy/refs/heads/main/vmbuddy.sh" | install -Dpm0755 /dev/stdin "${HOME}/.local/bin/vmbuddy"
```
