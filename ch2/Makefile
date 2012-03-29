DRIVER = hello

ifneq ($(KERNELRELEASE),)
	obj-m := $(DRIVER).o
else
	KERNELDIR ?= /lib/modules/$(shell uname -r)/build
	PWD := $(shell pwd)

default:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules

clean:
	rm -rf *.ko *.o *.mod.c modules.order Module.symvers .$(DRIVER)* .tmp_versions

endif

