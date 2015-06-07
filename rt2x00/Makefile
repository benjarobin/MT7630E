
mt7630pci-y	+= rt2x00dev.o
mt7630pci-y	+= rt2x00mac.o
mt7630pci-y	+= rt2x00config.o
mt7630pci-y	+= rt2x00queue.o
mt7630pci-y	+= rt2x00link.o
mt7630pci-y	+= mt_linux.o
mt7630pci-y	+= rt2x00crypto.o
mt7630pci-y	+= rt2x00firmware.o
mt7630pci-y	+= rt2x00leds.o
mt7630pci-y	+= rt2x00mmio.o
mt7630pci-y	+= rt2x00pci.o
mt7630pci-y	+= rt2800lib.o
mt7630pci-y	+= rt2800pci.o

obj-m		+= mt7630pci.o

KVERSION:= $(shell uname -r)

all:
	$(MAKE) -C /lib/modules/$(KVERSION)/build M=$(PWD) modules
clean:
	$(MAKE) -C /lib/modules/$(KVERSION)/build M=$(PWD) clean
