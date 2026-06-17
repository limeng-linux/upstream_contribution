# upstream_contribution
# Linux mainline upstream
fd8fca21629d dt-bindings: watchdog: fsl-imx-wdt: add compatible string fsl,ls1046a-wdt
720fd1cbc0a0 arm64: dts: add big-endian property back into watchdog node
7838de15bb70 usb: dwc3: core: remove lock of otg mode during gadget suspend/resume to avoid deadlock
486a64b29c5f watchdog: core: stop watchdog when executing poweroff command
69bef19d6b97 gpiolib: cdev: Set lineevent_state::irq after IRQ register successfully
745fa3e40ff5 arm64: dts: fsl-ls1043a-rdb: add delay between CS and CLK signal for flash device
efd21e10fc3b crypto: caam - replace this_cpu_ptr with raw_cpu_ptr
911957003948 net: stmmac: socfpga: add runtime suspend/resume callback for stratix10 platform
dc7e5940aad6 soc: fsl: dpio: use the combined functions to protect critical zone
e775eb9fc2a4 soc: fsl: dpio: replace smp_processor_id with raw_smp_processor_id
56a1188159cb mfd: syscon: Free the allocated name field of struct regmap_config
ea94191e584b spi: cadence: set cqspi to the driver_data field of struct device
e41a962f82e7 regmap: set debugfs_name to NULL after it is freed
d0243bbd5dd3 drivers core: Free dma_range_map when driver probe failed
56d9e7bd3fa0 EDAC/altera: Use fast register IO for S10 IRQs
#	u-boot upstream
2f74cac8c32 net: fec_mxc: add DM_FLAG_ACTIVE_DMA flag for FEC network driver
04cc66c047d rpi: set the correct parameter for simple framebuffer node
28cd244e847 bcm2835: Add simiple-framebuffer for use with fkms
aed2ebaa1fa arm: socfpga: socfpga_stratix10: enable wdt command by default
4f7abafe1c6 driver: watchdog: reset watchdog in designware_wdt_stop() function
# meta-intel-fpga layer
645f681 layer.conf: add layer compatibility to hardknott
# meta-raspberrypi layer
c327598 u-boot: Remove the randundant patch
# meta-freescale layer
04c08b12 qe-ucode: replace NXP-Binary-EULA with LICENSE to calculate checksum
a43e9940 fmc: update patch format
7f2d7385 meta-freescale: improve parameter definition of function errorFuncHandler
60a057fd meta-freescale: tsntool: remove redundant parameters from BIN_LDFLAGS
abe22513 meta-freescale: fmlib: map kernel source path to target path
4d97ada2 imx-gpu-viv: inherit features_check in  imx-gpu-viv bb file
cceaf0bb fmlib: set precise BSD license
# meta-freescale-distro layer
ba24fa4 meta-freescale-distro: add necessary dependent layers for meta-freescale-distro
4050f49 packagegroup-fsl-gstreamer1.0: use corrtect plugin name
# meta-tegra layer
6021c660 standalone-mm-optee-tegra: fix shell syntax error in TEGRA_BUILD_GUID ()
d8f4c83a gstreamer1.0-plugins-nveglgles: create a patch to fix building issue ()
# meta-tegra-community layer
795ce68 deepstream-7.1: fix libjsoncpp SONAME mismatch
# nvidia-kernel-oot/nvdisplay repo
ebc5f87 nvdisplay: nvidia-drm: add constify attribute for struct drm_display_mode instance
1de3392 nvdisplay: nvidia-drm: remove unused date member
f9f7d88 nvdisplay: nvidia-drm: fb: add format info parameter to tegra fb API
cf383b7 nvdisplay: timer: replace del_timer_sync() with timer_delete_sync()
844974d nvdisplay: nvidia: check importer operations directly
ebc18b9 nvdisplay: timer: replace hrtimer_init() with hrtimer_setup()
6eb36c9 nvdisplay: kernel-open: correct parameter of macro MODULE_IMPORT_NS
# nvidia-kernel-oot/nvgpu repo
4fe778bab nvgpu: timer: replace hrtimer_init() with hrtimer_setup()
ea5ec6060 gpu: nvgpu: correct parameter of macro MODULE_IMPORT_NS
#	nvidia-kernel-oot/nvidia-oot repo
98b05768 sound: soc: replace of_property_read_bool() with of_property_present()
07f75859 drivers: mttcan: remove constify attribute for ttcan_read_ts_cntr()
2f5bd488 drivers: realtek: bt: replace set_bit() with hci_set_quirk()
57f1b2ad sound: soc: replace idle_bias_off with idle_bias
eae699ee sound: soc: use reasonable SND_SOC_DAIFMT_CBx_CFx
a9e83f7f crypto: tegra - Remove an incorrect iommu_fwspec_free() call in tegra_se_remove()
faee3a36 sound: soc: set Codec/Stream/Card name explicitly
3e39dbd9 drivers: nvmap: calculate page address explicitly
9047aeda drivers: crypto: add priv pointer in context struct to save request
#	linux-yocto upstream
=== v4.18-standard-intel-socfpga: 5 patches ===
  09b9ff9ca052 arch: arm64: dts: add altr,sysmgr-syscon property for
  c92855291799 arch: arm64: dts: add property snps,multicast-filter-bins for
  d0af3a68d41d arm64: dts: add dts for updating FPGA configure
  d544645d2235 intel-socfpga: dts: add rsu node to enable rsu driver
  4d70227e1ff4 intel-socfpga: dts: improve qspi node for rsu feature
=== v4.19-standard-xlnx-soc: 1 patches ===
  2dc1554d5f0f regmap: set debugfs_name to NULL after it is freed
=== v5.2-standard-bcm-2xxx-rpi: 6 patches ===
  b3ce39e30241 arch: arm64: dts: Set gpio5-pin9 as input by default
  69ce9ac46cd1 build/arm64: Add rules for .dtbo files for dts overlays
  ac2a0083d6d0 driver: bcm2835-dma: fix build warning
  ce97136a2f8e driver: net: can: disable clock when it is in enable status
  2dc0e061c8e0 driver: usb: otg: fix build warning
  687ae878843f Revert "arm64: dts: r8a7795: Add CPUIdle support for all CPU
=== v5.2-standard-xlnx-soc: 1 patches ===
  c9007a43debd driver: pcie: reset pcie device with MIO31 on xilinx-zcu102
=== v5.4-standard-bcm-2xxx-rpi: 16 patches ===
  8252009ac16a arch: arm64: dts: add clock property in bcm2838.dtsi
  579faa45a039 arch:arm: bcm2711: add reset controller for usb device
  efe867cce124 arch: arm: dts: remove redundant emmc2 node
  b62f580da601 driver: cpufreq: initialize variable 'rate'
  989a2b462641 driver: drm: vc4: fix a wrong parameter
  639aff659b7e driver: net: lan78xx: fix building issue introduced by
  5e3d53e6e62a drivers: staging: vc04_services: add VCHI_INSTANCE_T member
  467a1109f195 drivers: staging: vc04_services: remove the static keyword
  939af1989719 Revert "arch: arm: dts: remove redundant emmc2 node"
  84b5367f56a3 Revert "cgroup: Disable cgroup "memory" by default"
  3d39641d3055 Revert "media: bcm2835: unicam: add media controller support"
  1a116bedf718 Revert "media: bcm2835-unicam: Add support for enum
  1685673016a2 Revert "media: bcm2835-unicam: Driver for CCP2/CSI2 camera
  cbabfc40671e Revert "media: bcm2835-unicam: Pass through the colorspace on
  a5060f83eb8d Revert "media:bcm2835-unicam: Power on subdev on
  a73ea06d05d3 Revert "media: bcm2835: unicam: Reduce scope of local
=== v5.4-standard-nxp-s32g2xx: 1 patches ===
  d83bc7e42449 driver: regmap: set debugfs_name to NULL after it is freed
=== v5.7-standard-bcm-2xxx-rpi: 1 patches ===
  16330b9ff8f4 drivers: vc04_services: instead of VFL_TYPE_GRABBER with
=== v5.8-standard-bcm-2xxx-rpi: 3 patches ===
  e8fb10dfaa13 driver: net: lan78xx: fix building issue introduced by
  8191578c3514 drivers: staging: vc04_services: add vchiq instance member
  e50ad5938e28 drivers: staging: vc04_services: remove the useless static
=== v5.10-standard-bcm-2xxx-rpi: 18 patches ===
  62a372cd5012 arch: arm: dts: rename sdhci to mmc
  4f0762ac32b5 crypto: caam - replace this_cpu_ptr with raw_cpu_ptr
  1209195ed0f7 driver: adc: ltc2497: return directly after reading the adc
  3962e4150750 driver: gpu: vc4: fix building issue caused by upgrading
  2d0e663f63d8 driver: net: bcmgenet: remove useless code
  2f2f026d5112 driver: net: broadcom: restore bcm54213pe configuration
  938c2d442967 driver: of: remove the redundant OF_CONFIGFS item in Kconfig
  8cd3c48c1baf drivers core: Free dma_range_map when driver probe failed
  2ca0c98f9afb driver: thermal: thermal: fix build issue caused by merging
  049b00316cb1 driver: vc04_services: initialize queue_lock field of struct
  56d9e7bd3fa0 EDAC/altera: Use fast register IO for S10 IRQs
  657803b918e0 gpiolib: cdev: Set lineevent_state::irq after IRQ register
  f0a079c0ba87 mfd: syscon: Free the allocated name field of struct
  55c97165adf6 soc: fsl: dpio: replace smp_processor_id with
  7e867f8bb3fe soc: fsl: dpio: use the combined functions to protect
  422806f8d289 spi: cadence: set cqspi to the driver_data field of struct
  8731a0b180f6 usb: dwc3: core: remove lock of otg mode during gadget
  a8f317c1a17e yaffs: replace IS_ERR with IS_ERR_OR_NULL to check both ERR
=== v5.10-standard-intel-sdk-5.10-intel-socfpga: 25 patches ===
  4104155dd298 aarch: arm64: dts: add #clock-cells property in gmac node
  61f421e6c15d aarch: arm64: dts: add condition to include qse dtsi file
  6a8404980c2b arch: arm64: altera: add dts file to support gpio on FPGA
  efc5265ab54e arch: arm64: altera: add dts file to support sgmii ethernet
  443b4e71ea9a arch: arm64: dts: disable fcs feature by default on Intel
  03a19d447fbb arch: arm64: intel: add dts file to support FPGA update
  d336f049ea88 arch: arm64: intel: add dts file to support gpio on FPGA side
  ce48c8d912d6 arch: arm64: intel: add dts file to support sgmii ethernet on
  40cdb750ded8 arch: arm64: intel: create dts to support FPGA GPIO and SGMII
  27d90a2315b1 arm64: dts: enable qspi-nor flash for Agilex NAND booting
  73737294903a arm64: dts: intel: improve qspi node for rsu feature
  0eee61da3433 arm64: psci: don't create online interface file for cpu0 on
  ee00cf1ab1ab driver: edac: altera_edac: fix build warning
  618173d5a066 driver: edac: create an interface to check ecc feature status
  e27ebb471130 driver: ethernet: stmmac: remove the redundant clock disable
  aed966027aad drivers: spi: cadence: set cqspi to the driver_data field of
  4a5bf3b19c9d driver: stratix10-svc: correct the error processing path
  94415527742e firmware: stratix10-svc: release mutex sdm_lock after
  f4aa570827ad firmware: stratix10-svc: remove the code of adding intel-fcs
  cdf0bb9c6c69 i2c: altera: Enable Altera I2C driver for Stratix10
  9dfe713b6ff1 intel: fcs: avoid allocating memory repeatedly
  d5af53b52e3a intel: fcs: disable to request random number generation on
  00295d5977ed intel: fcs: release mutex lock in failing path
  78a246155dee mfd: altera-sysmgr: enable raw spinlock feature for
  f334424a2891 mtd: rawnand: denali_dt: start denali nand driver a little
=== v5.10-standard-nxp-sdk-5.10-nxp-s32g2xx: 1 patches ===
  da45b48c35e0 arch: arm64: dts: keep i2c1 in disabled status
=== v5.10-standard-nxp-sdk-5.10-nxp-soc: 9 patches ===
  68b6055d3be6 arch: arm64: dts: add delay between CS and CLK signal for
  85df6f077860 arch: arm64: dts: add dts files for nxp-ls1023 platform
  bcf9e14cd524 arch: arm64: dts: disable sec_jr2 dts node
  b1034f052c2b arm64: mm: add the code that is missed when upgrade kernel
  fc57380a82c4 driver: sdk_fman: remove the disable interrupt action in
  f920c1a17837 drivers: dpaa: Convert the rx_pool_channel_init from spinlock
  d06e30613683 drivers: staging: fsl_qbman: move used_node variable
  0c4c095efc32 driver: staging: fsl_qbman: avoid preempt disable action by
  8545cf4d28e6 driver: staging: fsl_qbman: improve PORTAL_IRQ_LOCK/UNLOCK()
=== v5.15-standard-bcm-2xxx-rpi: 8 patches ===
  af3cdb763fc0 arch: arm64: dts: remove the dts file with license limitation
  00cc139b1d7c drivers:drm:vc4: fix building issue caused by upgrading
  bb1d90ce738e drivers: wireless: brcmfmac: use correct interface to record
  87a0dc5d3ac8 drm: vc4_hdmi: use more accurate variable to replace
  a3dd211c1a49 Revert "drm: Introduce DRM_BRIDGE_OP_UPSTREAM_FIRST to alter
  681ee78ebc26 Revert "drm/tc358762: Set the DRM_BRIDGE_OP_UPSTREAM_FIRST
  45cb814d0f7a serial: pl011: fix building conflict caused by upgrading
  b5d500042eb3 usb: hcd-pci: remove the action of faking interrupt request
=== v5.15-standard-intel-sdk-5.15-intel-socfpga: 1 patches ===
  03428a923c27 arch: arm64: dts: improve the overlay used to updating FPGA
=== v5.15-standard-nxp-sdk-5.15-nxp-soc: 14 patches ===
  7349ba549bb7 arch: arm64: dts: add dts files for nxp-ls1026 platform
  60493c9d8694 arch: arm64: dts: set correct phy-connection-type for aqr107
  51b3c2cb9bd8 arm64: dts: ls1028a: correct the lane mapping property for
  2da5a9249a7d driver: net: dpaa: improve the assignment operation for
  8029db9b31c5 driver: net: dpaa: release resource when executing kexec
  292102216aa2 driver: net: dpaa: support interface mode usxgmii
  4954cdb8a519 drivers: enetc: tsn: free the CBS structure
  1df65ab9902a drvier: dpaa: Convert the rx_pool_channel_init from spinlock
  6c387e185e8f drvier: staging: fsl_qbman: move used_node variable
  44580aa8edd1 enetc: add suspend/resume function to manage pm in ethernet
  e435ffe85bae enetc: tsn: release resource before exiting
  b76d72651889 gpu: drm: bridge: improve the function of getting training
  21e47a90b95f tsn: replace GFP_KERNEL with GFP_ATOMIC to avoid sleeping in
=== v5.19-standard-bcm-2xxx-rpi: 1 patches ===
  745fa3e40ff5 arm64: dts: fsl-ls1043a-rdb: add delay between CS and CLK
=== v6.1-standard-bcm-2xxx-rpi: 1 patches ===
  abe363d6f953 media: i2c: imx219: align with stable kernel code
=== v6.1-standard-intel-sdk-6.1-intel-socfpga: 3 patches ===
  2b0d654c4682 intel-socfpga: dts: improve qspi nor-flash partitions for
  cb7302ef56c7 usb: dwc2: add new compatible for Intel SoCFPGA Stratix10
  5132317e2d7a watchdog: dw_wdt: register notify callback to stop watchdog
=== v6.1-standard-nxp-sdk-5.15-nxp-s32g: 1 patches ===
  d4e587ba6844 arch: arm64: dts: remove llce_boot_status node to avoid
=== v6.1-standard-nxp-sdk-6.1-nxp-soc: 9 patches ===
  3fa4da923720 clk: imx: fracn-gppll: add missing code introduced by
  193d9ab0e3e9 dmaengine: imx-sdma: move memory copy operation before dma
  c4355676c93c driver: net: dpaa: support AQR113C phy on revision C
  2fc50fc3cd5b driver: sdk_fman: move the irq free operation to the front of
  78b405987cd0 drivers: drm: cadence: select DRM_DISPLAY_HDMI_HELPER if
  7183ec732057 drivers: fsl_qbman: alloc memory with GFP_ATOMIC parameter
  061342be6f3e drivers: fsl_qbman: replace GFP_KERNEL with GFP_ATOMIC during
  3eb6fef164f3 drivers: i2c: remove default y from I2C_IMX_FLEXIO config
  5e1946ef5302 Revert "gpu: drm: bridge: improve the function of getting
=== v6.1-standard-preempt-rt-sdkv6.1-xlnx-soc: 1 patches ===
  e318b47db650 arch: arm64: dts: add dts file for CANFD feature on
=== v6.6-standard-nvidia-orin: 4 patches ===
  ff45677be1ab drivers: phy: realtek: fix building issue caused by merging
  fda722775019 drivers: phy: remove redundant code introduced by SDK kernel
  765796059914 PCI: tegra194: combine sdk patch with latest linux-stable
  1bec2b683afa Revert "Revert "PCI: endpoint: Add support in configfs to
=== v6.12-standard-bcm-2xxx-rpi: 2 patches ===
  a86ea423dc13 arm64: dts: add big-endian property back into watchdog node
  65ec4e55088d arm64: dts: enable cgroup memory controller for raspberrypi5
=== v6.12-standard-nvidia-sdk-5.15-nvidia-soc: 6 patches ===
  e135351d4c81 cpufreq: tegra194: avoid setting invalid cpu mask
  4779407e9a80 firmware: tegra: bpmp: improve the solution of protecting
  04d51f3a782b firmware: tegra: bpmp: remove unused variable
  62c214ba270b Kconfig: select MMU_NOTIFIER config for NVIDIA Orin platform
  ec168f327a66 soc/tegra: pmc: simulate interrupt environment before
  802154ed3abc spi: tegra114: Set the default unit for CS delays
=== v6.12-standard-nxp-sdk-6.12-nxp-soc: 4 patches ===
  95b80dc087b9 driver: net: dpaa: remove unsupported features for interface
  e217388940af drivers: media: enforce camera driver to be loaded before
  72c0eec0bb27 dt-bindings: watchdog: fsl-imx-wdt: add compatible string
  61166865b5b8 net: sdk_dpaa: select phylink feature for sdk dpaa ethernet
=== v6.18-standard-nvidia-soc: 1 patches ===
  5142f15c6922 serial: tegra-tcu: skip console write in kgdb debug context
