## archlinux

#### Download:
[Link text Here](https://link-url-here.org)

<pre>
Download torrent: https://archlinux.org/releng/releases/2023.01.01/torrent/

[Link text Here](https://link-url-here.org)

You get a torrent file like this:
archlinux-2023.01.01-x86_64.iso.torrent

Open torrent file in: transmission
</pre>

#### Make bootable usb:
<pre>
sudo dd bs=4M if=archlinux-2023.01.01-x86_64.iso of=/dev/sdb conv=fsync oflag=direct status=progress

</pre>
