# Ux500 Platform Support

ifdef CONFIG_SND_SOC_UX500_DEBUG
CFLAGS_u8500.o := -DDEBUG
CFLAGS_ux500_pcm.o := -DDEBUG
CFLAGS_ux500_msp_dai.o := -DDEBUG
CFLAGS_ux500_ab8500.o := -DDEBUG
CFLAGS_ux500_ab8540.o := -DDEBUG
CFLAGS_ux500_av8100.o := -DDEBUG
CFLAGS_ux500_cg29xx.o := -DDEBUG
CFLAGS_ux500_msp_i2s.o := -DDEBUG
endif

ifdef CONFIG_UX500_SOC_DBX500
snd-soc-ux500-platform-objs := ux500_pcm.o ux500_msp_dai.o ux500_msp_i2s.o
obj-y += snd-soc-ux500-platform.o
endif

ifdef CONFIG_SND_SOC_UX500_AB850X
snd-soc-ux500-machine-objs += ux500_ab8500.o
endif

ifdef CONFIG_SND_SOC_UX500_AB8540
snd-soc-ux500-machine-objs += ux500_ab8540.o
endif

ifdef CONFIG_SND_SOC_UX500_AV8100
snd-soc-ux500-machine-objs += ux500_av8100.o
endif

ifdef CONFIG_SND_SOC_UX500_CG29XX
snd-soc-ux500-machine-objs += ux500_cg29xx.o
endif

obj-y += snd-soc-ux500-machine.o

ifdef CONFIG_UX500_SOC_DB8500
snd-soc-u8500-objs := u8500.o
obj-y += snd-soc-u8500.o
endif
