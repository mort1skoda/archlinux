## archlinux

#### Download:
[archlinux.org/download](https://archlinux.org/download/)

<pre>
You get a torrent file like this:
archlinux-2023.01.01-x86_64.iso.torrent

Open torrent file in: transmission
And download the .iso file
</pre>

#### Make bootable usb:
<pre>
sudo dd bs=4M if=archlinux-2023.01.01-x86_64.iso of=/dev/sdb conv=fsync oflag=direct status=progress
</pre>

[Installation guide](https://wiki.archlinux.org/title/Installation_guide)

<pre>
loadkeys no

To verify the boot mode, list the efivars directory:
ls /sys/firmware/efi/efivars
   If the command shows the directory without error,
   then the system is booted in UEFI mode.

ip link
ping -c 4 archlinux.org

   Note: In the installation image, systemd-networkd, systemd-resolved,
   iwd and ModemManager are preconfigured and enabled by default.
   That will not be the case for the installed system.

timedatectl status


</pre>


