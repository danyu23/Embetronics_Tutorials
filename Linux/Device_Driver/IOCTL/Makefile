obj-m += driver.o
 
KDIR ?= /lib/modules/$(shell uname -r)/build
 
 
all:
	make -C $(KDIR)  M=$(shell pwd) modules

modules_install:
	$(MAKE) -C $(KDIR) M=$(shell pwd) modules_install
 
clean:
	make -C $(KDIR)  M=$(shell pwd) clean
