```
# dependencies
sudo apt update && sudo apt upgrade
sudo apt-get install ninja-build gettext cmake curl build-essential
sudo apt install unzip
sudo apt install zsh
sudo apt install gh

# neovim
git clone https://github.com/neovim/neovim
cd neovim
git checkout stable
make CMAKE_BUILD_TYPE=RelWithDebInfo
sudo make install
git clone https://github.com/gica4343/neovim.config.git ~/.config/nvim

# tmux
git clone https://github.com/gica4343/tmux.config.git
cd tmux.config
mv .tmux.conf /home/$USER
cd && rm -rf tmux.config/

# omz
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# zsh
git clone https://github.com/gica4343/zshrc.git
cd zshrc
cp .zshrc ~ && cd ~

# sleep
git clone https://github.com/gica4343/linux-setup.git && cd linux-setup/
sudo cp disable-some-wake /usr/lib/systemd/system-sleep
sudo chmod 755 /usr/lib/systemd/system-sleep/disable-some-wake
cd
```
