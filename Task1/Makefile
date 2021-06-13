obj-m += Task1.o

KDIR = /lib/modules/$(shell uname -r)/build

PWD = $(shell pwd)

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules
install:
	$(MAKE) -C $(KDIR) M=$(PWD) modules_install
%:
	$(MAKE) -C $(KDIR) M=$(PWD) $@
