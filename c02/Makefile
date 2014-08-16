obj-m := hello.o
module-objs := hello.c

# for arm board
# CC=arm-linux-gcc
# KERNEL_DIR=/home/archer/code/linux-2.6.32.2

# for my pc
CC=gcc
KERNEL_DIR=/lib/modules/3.13.0-24-generic/build

default:
	make -C ${KERNEL_DIR} M=`pwd` modules


clean:
	rm -rf *.o
	rm -rf *.ko
	rm -rf *.order
	rm -rf *.symvers
	rm -rf .*.cmd
	rm -rf *.mod.c
	rm -rf .tmp_versions
