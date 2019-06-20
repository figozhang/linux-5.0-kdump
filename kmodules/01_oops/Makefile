BASEINCLUDE ?= /lib/modules/$(shell uname -r)/build

oops-objs := oops_test.o 
KBUILD_CFLAGS +=-g -O0


obj-m	:=   oops.o
all : 
	$(MAKE) -C $(BASEINCLUDE) M=$(PWD) modules;

install:
	$(MAKE) -C $(BASEINCLUDE) M=$(PWD) modules_install;
	
	

clean:
	$(MAKE) -C $(BASEINCLUDE) M=$(PWD) clean;
	rm -f *.ko;


