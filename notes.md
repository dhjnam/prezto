For some reasons (likely due to proper setting of certain environment
variables) it is not enough to have `dhjnam/prezto.git` here in the
 `~/.config` folder and then symlinking the startup files from the home
folder.

```sh
ln -s ~/.config/zsh/prezto/runcoms/zlogin ~/.zlogin
ln -s ~/.config/zsh/prezto/runcoms/zlogout ~/.zlogout
ln -s ~/.config/zsh/prezto/runcoms/zpreztorc ~/.zpreztorc
ln -s ~/.config/zsh/prezto/runcoms/zprofile ~/.zprofile
ln -s ~/.config/zsh/prezto/runcoms/zshenv ~/.zshenv
ln -s ~/.config/zsh/prezto/runcoms/zshrc ~/.zshrc
```

To trick the operating system in believing that `~/.zprezto` has been
installed in the home folder, we must create a symlink to this project

```sh
ln -s ~/.config/zsh/prezto ~/.zprezto
```

This way there will not be any issues with environment variables
