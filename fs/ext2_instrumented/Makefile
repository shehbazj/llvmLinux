obj-m += ext2.o

ext2-objs := all.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) all.o
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) ext2.ko

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
	rm *.S *.bc
