# Personal zed config

## Initial setup

Repo was created to track zed settings & keybindings.

Initial setup:

```
mkdir zed-config
cd zed-config
git init
cp ~/.config/zed/settings.json .
cp ~/.config/zed/keymap.json .
git remote add origin https://github.com/clemsau/zed-config.git
git add .
git commit -m "Initial Zed config"
git push -u origin main
```

Then, symlink creation:

```
ln -sf zed-config/settings.json ~/.config/zed/settings.json
ln -sf zed-config/keymap.json ~/.config/zed/keymap.json
```

## Copying the settings locally

> [!CAUTION]
> This will override the local zed configs. Be sure to have a backup if necessary.

Clone the repo:

```
git remote add origin git@github.com:clemsau/zed-config.git
```

Go in the repo, and create the symlinks:

```
cd zed-config
ln -sf settings.json ~/.config/zed/settings.json
ln -sf keymap.json ~/.config/zed/keymap.json
```

## Maintenance

Just push from this repo whenever settings or keybindings are modified locally.

Pull from this repo regularly, especially when you know settings or keybindings has been modified.
