#
# USB peripheral controller drivers
#
# Use the BUS_INTERFACE variable to compile the software for either 
# PCI(PCI_INTERFACE) or LM(LM_INTERFACE) bus.
# Use one of the following flags to compile the software in host-only or
# device-only mode.
EXTRA_CFLAGS        += -DDWC_DEVICE_ONLY
EXTRA_CFLAGS		+= -DDWC_LINUX
EXTRA_CFLAGS		+= -DLM_INTERFACE

obj-$(CONFIG_HI_HS_DEVICE)	+= dwc_otg.o
dwc_otg-objs	:= dwc_otg_driver.o dwc_otg_attr.o 
dwc_otg-objs	+= dwc_otg_cil.o dwc_otg_cil_intr.o 
dwc_otg-objs	+= dwc_otg_pcd_linux.o dwc_otg_pcd.o dwc_otg_pcd_intr.o 
dwc_otg-objs	+= dwc_otg_hcd.o dwc_otg_hcd_linux.o dwc_otg_hcd_intr.o dwc_otg_hcd_queue.o dwc_otg_hcd_ddma.o
dwc_otg-objs	+= dwc_otg_adp.o
dwc_otg-objs	+= dwc_cc.o dwc_modpow.o dwc_dh.o \
			    dwc_crypto.o dwc_notifier.o \
			    dwc_common_linux.o dwc_mem.o





