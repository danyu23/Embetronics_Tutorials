obj-m += hello_world.o
 
KERNEL_SRC = "/lib/modules/$(shell uname -r)/build"

all:
	$(MAKE) -C $(KERNEL_SRC)  M=$(shell pwd)
	
modules_install:

	$(MAKE) -C $(KERNEL_SRC) M=$(shell pwd) modules_install
 
clean:
	make -C $(KERNEL_SRC)  M=$(shell pwd) clean
