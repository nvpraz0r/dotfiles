# dotfiles

This is my script for setting up my development environment. You can use it yourself, too. It won't bite!

I've tried to make the default setup as non-custom as possible while still providing sensible defaults for developers.

But, of course, a lot of this still caters to my tastes. :)

## Installation

Pick master or bissell:

Master: `git clone -b master git@github.com:kibiz0r/dotfiles.git ~/.dotfiles && cd ~/.dotfiles && ./install`
BISSELL: `git clone -b bissell git@github.com:kibiz0r/dotfiles.git ~/.dotfiles && cd ~/.dotfiles && ./install`

If you want the kibiyama awesomesauce, run `./install_plus_kibiyama` instead of `./install`.

## Customization

You can layer your own stuff on top of the base stuff. If you use the kibiyama stuff, your stuff will be run last so you don't get overwritten.

To understand what's going on, look at `install.conf.yaml`.

There are some environment variables you can change to tailor the installation to your environment.

```
USE_VSCODE_INSIDERS to use bleeding-edge VSCode
USE_SUDO to do full setup rather than non-admin captive setup
USE_HOME_APPDIR to cheat and install apps to ~/Applications (mainly to avoid getting admin permissions to run stuff)
USE_HOME_HOMEBREW to install Homebrew to ~/homebrew... Try not to use this one if you can help it
USE_KIBIYAMA_CUSTOMIZATIONS to use my custom configs
```

The default setup is rather idealistic and safe. It uses stable VSCode, avoids sudo, installs to global /Applications, installs Homebrew normally, and doesn't use my custom stuff.
