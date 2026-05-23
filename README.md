<p align="center">
  <img src="kiro.jpg" alt="Kiro" width="220" />
</p>

# edu-plasma-keybindings

Erik's KDE Plasma keyboard-shortcut customisations, shipped as a dotfile drop-in. Part of the `~/EDU/` learning series — drop these in and your Plasma session inherits the Kiro-flavour bindings.

## What's in this repo

- `etc/skel/` — Plasma's `kglobalshortcutsrc` (and related config) that lands in `/etc/skel/`.
- `setup.sh`, `up.sh` — standard EDU bash scaffold.

## Installation

### From `nemesis_repo` (recommended)

```ini
[nemesis_repo]
SigLevel = Never
Server = https://erikdubois.github.io/$repo/$arch
```

```bash
sudo pacman -Syu
sudo pacman -S edu-plasma-keybindings-git
```

### Manual

```bash
git clone https://github.com/erikdubois/edu-plasma-keybindings.git
cd edu-plasma-keybindings
sudo cp -r etc/skel/. /etc/skel/
```

Existing users can copy directly into their own home:

```bash
cp -rT /etc/skel ~/
```

Plasma re-reads `kglobalshortcutsrc` on login — log out and back in to pick up the new bindings.

## Websites

Information : https://erikdubois.be

## Social Media

Youtube : https://www.youtube.com/erikdubois

## License

See [LICENSE](./LICENSE).
