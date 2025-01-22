```
# neovim
git clone https://github.com/gica4343/neovim.config.git ~/.config/nvim

# tmux
git clone https://github.com/gica4343/tmux.config.git
cd tmux.config
mv .tmux.conf /home/$USER
cd && rm -rf tmux.config/

# zsh
git clone https://github.com/gica4343/zshrc.git
cd zshrc
cp .zshrc ~ && cd ~

# sleep
sudo cp disable-some-wake /usr/lib/systemd/system-sleep
sudo chmod 755 /usr/lib/systemd/system-sleep/disable-some-wake
```
