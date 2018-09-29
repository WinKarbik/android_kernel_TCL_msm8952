dtb-$(CONFIG_ARCH_VEXPRESS) += rtsm_ve-aemv8a.dtb foundation-v8.dtb
dtb-$(CONFIG_ARCH_XGENE) += apm-mustang.dtb

targets += dtbs

#used for cleaning - not building
ifndef CONFIG_TCT_8X76_COMMON
subdir- := dts/qcom
endif

ifdef CONFIG_TCT_8X76_IDOL4
subdir- := dts/idol4
endif

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := dts/*.dtb *.dtb
