#
# Makefile
#

all: prepare
	# Run Linux Kernel with Alpine mini rootfs
	qemu-system-x86_64 -kernel linux-5.4.34/arch/x86/boot/bzImage -initrd rootfs.img -nographic -append "console=ttyS0"

prepare:
	./auto-tasks.sh

clean:
	rm -rf linux-5.4.34  
	rm -rf alpine-minirootfs-3.19.1-x86_64