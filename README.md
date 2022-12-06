# Replaceable MiniOS kernels.
This repository contains the kernels, initrds, and kernel modules needed to boot MiniOS.

To install the desired kernel, download the required vmlinuz, initrd and module. Place the module in the minios folder and vmlinuz and initrfs.img in the minios/boot folder. Delete the old vmlinuz and initrfs.img and rename the copied ones to vmlinuz and initrfs.img.

For kernels 5.10 and above:

X.X.X-X kernels (eg 5.10.0-19) are the original Debian kernels. They do not support AUFS, but they do support SecureBoot.

X.X.X-mos kernels (eg 5.10.149-mos) are kernels that we build from Debian configs with AUFS support.

For kernels 4.19 and below:

The original Debian kernels are used, supporting both AUFS and SecureBoot.