# 目标模块文件名（hello.o 最终变成 hello.ko）
obj-m += hello.o

# 内核构建树路径
KDIR := /lib/modules/$(shell uname -r)/build
# 当前目录
PWD := $(shell pwd)

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules

clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean
