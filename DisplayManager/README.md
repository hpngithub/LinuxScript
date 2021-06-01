# DISPLAY MANAGER
*NOTE : Below GUI Desktop Displaymananger for linux will install with packages as shown below. 
!! Add packages based on desktop selection.!!

	mate-Ubuntu)
		PACKAGES+=(
			ubuntu-mate-desktop
			ubuntu-mate-wallpapers
			ubuntu-mate-artwork
			mate-applet-brisk-menu
			mate-applet-appmenu
			mate-desktop-environment
			mate-desktop-environment-extra
			mate-desktop-environment-extras
			mate-dock-applet
			mate-menu
			mate-sensors-applet
			mate-tweak
			mate-user-share
			mate-system-monitor
			mate-user-guide
			mate-calc
			mate-accessibility-profiles
			mate-netbook
			mate-window-menu-applet
			mate-window-title-applet
			mate-hud
			network-manager
			network-manager-gnome
			network-manager-openvpn-gnome
			lightdm
			lightdm-gtk-greeter
			ubuntu-mate-lightdm-theme
			unity-greeter
			dconf-editor
		)
		;;

	mate-Debian)
		PACKAGES+=(
			mate-desktop-environment
			mate-desktop-environment-extra
			mate-desktop-environment-extras
			mate-hud
			mate-dock-applet
			mate-menu
			mate-sensors-applet
			mate-tweak
			mate-user-share
			mate-system-monitor
			mate-user-guide
			mate-calc
			mate-accessibility-profiles
			mate-netbook
			mate-window-menu-applet
			mate-window-title-applet
			desktop-base
			dconf-editor
			lightdm
			lightdm-gtk-greeter
		)
		;;

	gnome-Ubuntu)
		PACKAGES+=(
			ubuntu-gnome-desktop
			ubuntu-gnome-wallpapers-xenial
			gdm3
		)
		;;

	gnome-Debian)
		PACKAGES+=(
			gnome
			desktop-base
		)
		;;

	i3-Ubuntu|i3-Debian)
		PACKAGES+=(
			i3
			i3status
			i3lock
			slim
			rxvt-unicode-lite
		)
		;;

	xfce4-Ubuntu)
		PACKAGES+=(
			xubuntu-desktop
			lightdm
			lightdm-gtk-greeter
			ubuntu-mate-lightdm-theme
		)
		;;

	lxde-Ubuntu)
		PACKAGES+=(
			lxde
			lightdm
			lightdm-gtk-greeter
			ubuntu-mate-lightdm-theme
			slick-greeter
			network-manager
			network-manager-gnome
			network-manager-openvpn-gnome
		)
		;;

	lxde-Debian)
		PACKAGES+=(
			lxde
			lightdm
			lightdm-gtk-greeter
		)
		;;

	kde-Ubuntu)
		PACKAGES+=(
			kubuntu-desktop
			lightdm
			lightdm-gtk-greeter
		)
		;;

	*)

## InstallDesktop.sh = Install using below command desktop for ubuntu and Debain only.

          Command :
           
           - wget -O InstallDesktop.sh "https://raw.githubusercontent.com/hpngithub/LinuxScript/main/DisplayManager/InstallDesktop.sh" 
           - chmod a+x ./InstallDesktop.sh
           - ./InstallDesktop.sh <mate|i3|gnome|xfce4|lxde|kde>

### REFERENCES URL
- https://github.com/ayufan-rock64/linux-package/blob/master/root/usr/local/sbin/install_desktop.sh
- https://askubuntu.com/questions/799365/can-not-run-a-script-downloaded-with-wget-o-filename-sh-url
