# My custom configuration of MacOs

## How to setup this configuration

```shell
echo "source ~/MacosConfiguration/shell_config" >> ~/.zshrc
ln -sf "$HOME/MacosConfiguration/shell_config" ~/.config/fish/conf.d/shell_config.fish
ln -sf "$HOME/MacosConfiguration/alacritty.yml" ~/.config/alacritty/alacritty.yml
ln -sf "$HOME/MacosConfiguration/.tmux.conf" ~/.tmux.conf
```