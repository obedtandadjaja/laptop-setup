# laptop-setup
Setting up my mac

## Mac

### Font

1. Download `Source Code Pro` from [https://fonts.google.com/specimen/Source+Code+Pro?selection.family=Source+Code+Pro](https://fonts.google.com/specimen/Source+Code+Pro?selection.family=Source+Code+Pro)
2. Unzip the folder
3. Double click `Source Code Pro` and install the font

### Trackpad

1. Go to My Preferences
2. Go to Trackpad
3. Click `one tap to click`

### Keyboard

1. Go to My Preferences
2. Go to Keyboard
3. Click Modifier keys
4. Change `capslock` to `escape`

## iTerm2

1. Download iTerm2: [https://www.iterm2.com/](https://www.iterm2.com/)
2. Go to `Preferences`
3. Go to `Profile`
4. Choose `Esc+` for the left and right command key
5. Go to `Text`
6. Choose `Source Code Pro` for both fonts
7. Download ayu theme: [https://iterm2colorschemes.com/](https://iterm2colorschemes.com/)
8. Go to `Colors`
9. Click `color presets`, choose `import`, and choose the downloaded `ayu`
10. Go to `Terminal`
11. Click `Unlimited scrollback`

## emacs / spacemacs

1. `brew tap d12frosted/emacs-plus`
2. `brew install emacs-plus`
3. `ln -s /usr/local/Cellar/emacs-plus/*/Emacs.app/ /Applications/` create softlink for emacs in Applications
4. `git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d`
5. Get `.spacemacs` from [https://github.com/obedtandadjaja/dotfiles](https://github.com/obedtandadjaja/dotfiles)
6. Launch emacs `emacs --insecure`

## Postgres

1. Download the `Postgres.app` here: [https://postgresapp.com/](https://postgresapp.com/)
2. Move to Applications folder
3. Click `Initialize` to create a new server
4. Configure `$PATH` to use command line tools (optional): 
```
sudo mkdir -p /etc/paths.d &&
echo /Applications/Postgres.app/Contents/Versions/latest/bin | sudo tee /etc/paths.d/postgresapp
```

**Default settings:**

Host: `localhost`

Port: 5432

User: *System user name*
  
Database: *System user name*
  
Password: *none*
  
Connection URL: `postgresql://localhost`
