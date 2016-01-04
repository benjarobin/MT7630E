
mt7630e-y	+= rt2x00dev.o
mt7630e-y	+= rt2x00mac.o
mt7630e-y	+= rt2x00config.o
mt7630e-y	+= rt2x00queue.o
mt7630e-y	+= rt2x00link.o
mt7630e-y	+= mt_linux.o
mt7630e-$(CONFIG_RT2X00_LIB_CRYPTO)	+= rt2x00crypto.o
mt7630e-$(CONFIG_RT2X00_LIB_FIRMWARE)	+= rt2x00firmware.o
mt7630e-$(CONFIG_RT2X00_LIB_LEDS)	+= rt2x00leds.o
mt7630e-y	+= rt2x00mmio.o
mt7630e-y	+= rt2x00pci.o
mt7630e-y	+= rt2800lib.o
mt7630e-y	+= rt2800pci.o

obj-m		+= mt7630e.o

KERNELRELEASE ?= $(shell uname -r)
KDIR ?= /lib/modules/$(KERNELRELEASE)/build

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules
clean:
	$(MAKE) -C $(KDIR) M=$(PWD) clean
