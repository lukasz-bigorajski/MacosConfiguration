# My custom configuration of MacOs

## How to setup this configuration

```shell
echo "source ~/MacosConfiguration/shell_config" >> ~/.zshrc
ln -sf "$HOME/MacosConfiguration/shell_config" ~/.config/fish/conf.d/shell_config.fish
ln -sf "$HOME/MacosConfiguration/alacritty.yml" ~/.config/alacritty/alacritty.yml
ln -sf "$HOME/MacosConfiguration/.tmux.conf" ~/.tmux.conf
```

## FreeBSD vs GNU

MacOs is not based on Linux and therefore has several programs that are not compatible with these Linux counterparts. MacOs uses FreeBSD libraries and Linux uses GNU libraries. To be compatible with Linux libraries, the GNU libraries must be installed and override those already installed. This can be done with adding library path to PATH variable, fe. `export PATH="$(brew --prefix)/opt/gnu-sed/libexec/gnubin:$PATH"`

https://gist.github.com/skyzyx/3438280b18e4f7c490db8a2a2ca0b9da
