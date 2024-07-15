## upgrade the system
```bash
sudo pacman -Syu
```
```bash
yay -Syu
```
## remove the plank
```bash
yay -Rns plank
```
## install base-devel
```bash
yay -S base-devel
```
## install ohmyzsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
## install powerlevel10k
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k && source ~/.zshrc
```
if need to to re config
```bash
p10k configure
```
## install drakula theme in terminator
```bash
git clone https://github.com/dracula/terminator.git && cd terminator && ./install.sh
```
## install applications using yay
```bash
yay -S brave-bin btop kdeconnect android-studio-bin jdk17-openjdk \
brightness-controller dolphin gwenview logo-ls stacer-bin docker visual-studio-code-bin \
nvtop libxcrypt-compat github-cli coolercontrol lm-sensor nbfc-linux \
gwenview tlp preload tuned neofetch geekbench
```
## install application using pacman 

```bash
sudo pacman -S qemu-full qemu-img libvirt virt-install dnsmasq virt-manager virt-viewer edk2-ovmf swtpm guestfs-tools libosinfo \
openbsd-netcat ebtables iptables libguestfs virt-viewer dnsmasq vde2 bridge-utils \
noto-fonts noto-fonts-cjk ttf-dejavu ttf-liberation ttf-opensans
```
## install nodejs using nvm

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```
```bash
source ~/.zshrc && nvm install --lts
```
## install gnome
```bash
sudo pacman -S xorg xorg-server gnome 
