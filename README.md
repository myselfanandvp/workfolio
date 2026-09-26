# Workfolio for Arch Linux

Arch Linux package for **Workfolio Desktop**.

## Installation

Clone the repository:

```bash
git clone https://github.com/myselfanandvp/workfolio.git
cd workfolio
```

Build the Arch package:

```bash
makepkg -s
```

This will generate a package similar to:

```text
workfolio-0.1.54-1-x86_64.pkg.tar.zst
```

### Install with `yay`

```bash
yay -U workfolio-0.1.54-1-x86_64.pkg.tar.zst
```

Or install directly with `pacman`:

```bash
sudo pacman -U workfolio-0.1.54-1-x86_64.pkg.tar.zst
```

## Cleanup

After the installation is complete, you can remove the cloned repository and build files:

```bash
cd ..
rm -rf workfolio
```

The Workfolio application will remain installed on your system.

## Uninstall

To remove Workfolio:

```bash
sudo pacman -R workfolio
```

Or:

```bash
yay -R workfolio
```

## Requirements

* Arch Linux or an Arch-based distribution
* `base-devel`
* `git`
* `pacman` / `yay`

If `base-devel` and `git` are not installed:

```bash
sudo pacman -S --needed base-devel git
```

## Package Information

| Package        | Version        |
| -------------- | -------------- |
| Name           | Workfolio      |
| Version        | 0.1.54         |
| Architecture   | x86_64         |
| Package format | `.pkg.tar.zst` |
| License        | Custom         |

## Repository

[GitHub Repository](https://github.com/myselfanandvp/workfolio?utm_source=chatgpt.com)
