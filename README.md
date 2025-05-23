# dotfiles
My Nix [home-manager](https://github.com/nix-community/home-manager) configurations. 

## Dependencies
The sway window manager chrashes if installed with Nix. I couldn't fix it because of some limitations with the Nix home-manager that don't exist with NixOS. So for now it has to be installed separately. Instructions:

<details><summary>Debian Based</summary>

```
sudo apt install sway
```
</details>
<details><summary>Arch Based</summary>

```
sudo pacman -S sway
```
</details>

## Installation
```bash
# Just clone recursively
git clone --recursive https://github.com/MarkelCA/dotfiles.git
```
## Usage

```bash
# Personal profile
home-manager switch --flake ~/dotfiles/nix#markel
```
```bash
# Work profile
home-manager switch --flake ~/dotfiles/nix#work
```
---
Took inspiration from:
- [vimjoyer](https://github.com/vimjoyer)
- [ornicar](https://github.com/ornicar)
- [Smona](https://github.com/Smona)
