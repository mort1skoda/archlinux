## archlinux
### UEFI system  Learn Linux TV

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
To install via ssh:
ssh -o StrictHostKeyChecking=no -o "UserKnownHostsFile /dev/null" root@192.168.0.198
</pre>

<pre>
Start installing:
=================
loadkeys no
alias l='ls -la --color --group-directories-first'

