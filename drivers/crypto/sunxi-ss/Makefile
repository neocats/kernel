obj-$(CONFIG_CRYPTO_DEV_SUN4I_SS) += sun4i-ss.o
sun4i-ss-y += sun4i/sun4i-ss-core.o sun4i/sun4i-ss-hash.o sun4i/sun4i-ss-cipher.o

obj-$(CONFIG_CRYPTO_DEV_SUNXI) += ss.o

ss-y += sunxi_ss.o sunxi_ss_proc_comm.o

ifdef CONFIG_ARCH_SUN8IW11
	SUNXI_SS_VER = v3
endif
ifdef CONFIG_ARCH_SUN8IW12
	SUNXI_SS_VER = v3
endif
ifdef CONFIG_ARCH_SUN8IW15
	SUNXI_SS_VER = v3
endif

ss-y +=  $(SUNXI_SS_VER)/sunxi_ss_reg.o $(SUNXI_SS_VER)/sunxi_ss_proc.o

ccflags-y += -Idrivers/crypto/sunxi-ss/$(SUNXI_SS_VER)

#ccflags-y += -DDEBUG
