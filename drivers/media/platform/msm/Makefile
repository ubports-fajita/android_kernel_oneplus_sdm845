#
# Makefile for the qti specific video device drivers
# based on V4L2.
#
obj-$(CONFIG_MSM_VIDC_V4L2) += vidc/
obj-$(CONFIG_MSM_VIDC_3X_V4L2) += vidc_3x/
obj-y += sde/
ifeq ($(CONFIG_SPECTRA2_CAMERA), y)
obj-$(CONFIG_SPECTRA_CAMERA) += camera_v3/
else ifeq ($(CONFIG_ONEPLUS_DIR_CAMERA),y)
obj-$(CONFIG_SPECTRA_CAMERA) += camera_oneplus/
else
obj-$(CONFIG_SPECTRA_CAMERA) += camera/
endif
ifeq ($(CONFIG_ONEPLUS_DIR_CAMERA),y)
obj-$(CONFIG_MSMB_CAMERA) += camera_oneplus_v2/
else
obj-$(CONFIG_MSMB_CAMERA) += camera_v2/
endif
obj-y += broadcast/
obj-$(CONFIG_DVB_MPQ) += dvb/
obj-$(CONFIG_QCA402X) += qca402/
