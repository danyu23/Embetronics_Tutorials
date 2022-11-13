obj-m += hello_world.o
 
 
all:
	$(MAKE) -C $(KERNEL_SRC)  M=$(shell pwd)
	
modules_install:

	$(MAKE) -C $(KERNEL_SRC) M=$(shell pwd) modules_install
 
clean:
	make -C $(KDIR)  M=$(shell pwd) clean
