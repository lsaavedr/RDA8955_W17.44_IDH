## Makefile automatically generated by NewTest.pl ##
# For more information on the different variables, and others you
# may define, see $(SOFT_DIR)/Makefile.skel and/or read the doc
## --------------Don't change the line below------------------ ##
include $(SOFT_WORKDIR)/env/compilation/compilevars.mk

LOCAL_NAME := toolpool/8955/bl_ddr_check

LOCAL_API_DEPENDS := \
    platform \
    platform/base/common \
    platform/chip/defs \
    platform/edrv/aud \
    platform/edrv/pmd \
    platform/chip/regs/$(CT_ASIC)

LOCAL_MODULE_DEPENDS := \
    platform/chip/bootloader

IS_ENTRY_POINT := yes
BOOTLOADER := yes


LOCAL_EXPORT_FLAG += BOOTLOADER


# We always want to compile the flash programmer as a Ramrun.
export CT_RAMRUN := 1

# Do not include ROM content in the final elf file
export ROM_IN_FLASH_ELF := 0

# Do not generate BCPU image
export NO_BCPU_IMAGE := 1

# Special linker to get everything in internal sram.
LINKER_MASTER := blramrun.ld

C_SRC := $(wildcard *.c)
S_SRC := $(wildcard *.S)

include $(SOFT_WORKDIR)/env/compilation/compilerules.mk
