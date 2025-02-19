```
# dependencies
sudo apt update && sudo apt upgrade
sudo snap install nvim --classic
sudo apt install build-essential
sudo apt install unzip
sudo apt install zsh

# neovim
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
