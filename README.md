# Personal zed config

> [!NOTE]  
> Double check the commands and especially the path, as they need absolute

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
ln -sf ~/Github/zed-config/settings.json ~/.config/zed/settings.json
ln -sf ~/Github/zed-config/keymap.json ~/.config/zed/keymap.json
```

## Copying the settings locally

> [!CAUTION]
> This will override the local zed configs. Be sure to have a backup if necessary.

Clone the repo:

```
git remote add origin git@github.com:clemsau/zed-config.git
```

Create the symlinks:

```
ln -sf ~/Github/zed-config/settings.json ~/.config/zed/settings.json
ln -sf ~/Github/zed-config/keymap.json ~/.config/zed/keymap.json
```

## Maintenance

Just push from this repo whenever settings or keybindings are modified locally.

Pull from this repo regularly, especially when you know settings or keybindings has been modified.
