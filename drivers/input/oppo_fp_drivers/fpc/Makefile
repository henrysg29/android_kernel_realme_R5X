ifeq ($(CONFIG_OPPO_FINGERPRINT_QCOM),y)
ifeq ($(CONFIG_PRODUCT_REALME_RMX1911),y)
PROJECT_NAME = 19631
else ifeq ($(CONFIG_PRODUCT_REALME_RMX2030),y)
PROJECT_NAME = 19743
endif
endif

DEFS = -DCONFIG_OPPO_FINGERPRINT_PROJCT=$(PROJECT_NAME)
ccflags-y += $(DEFS)

DEFS = -DCONFIG_OPPO_FINGERPRINT_KERNEL_VER=$(VERSION)
ccflags-y += $(DEFS)

ifeq ($(CONFIG_OPPO_FINGERPRINT_QCOM),y)
obj-y  += fpc1020_tee.o
endif
