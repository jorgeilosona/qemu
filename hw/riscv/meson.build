riscv_ss = ss.source_set()
riscv_ss.add(files('boot.c'))
riscv_ss.add(when: 'CONFIG_HART', if_true: files('riscv_hart.c'))
riscv_ss.add(when: 'CONFIG_OPENTITAN', if_true: files('opentitan.c'))
riscv_ss.add(when: 'CONFIG_RISCV_VIRT', if_true: files('virt.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE', if_true: files('sifive_clint.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE', if_true: files('sifive_gpio.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE', if_true: files('sifive_plic.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE', if_true: files('sifive_test.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE', if_true: files('sifive_uart.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE_E', if_true: files('sifive_e.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE_E', if_true: files('sifive_e_prci.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE_U', if_true: files('sifive_u.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE_U', if_true: files('sifive_u_otp.c'))
riscv_ss.add(when: 'CONFIG_SIFIVE_U', if_true: files('sifive_u_prci.c'))
riscv_ss.add(when: 'CONFIG_SPIKE', if_true: files('riscv_htif.c'))
riscv_ss.add(when: 'CONFIG_SPIKE', if_true: files('spike.c'))

hw_arch += {'riscv': riscv_ss}
