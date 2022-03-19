# qemu

Install QEMU:
```bash
brew install qemu
```

Convert `qcow2` to `vhd`:
```bash
qemu-img convert -O vpc \
  Rocky-8-GenericCloud-8.5-20211114.2.x86_64.qcow2 \
  Rocky-8-GenericCloud-8.5-20211114.2.x86_64.vhd
```


Image format | Argument to qemu-img
---|---
QCOW2 (KVM, Xen) | qcow2
QED (KVM) | qed
raw | raw
VDI (VirtualBox) | vdi
VHD (Hyper-V) | vpc
VMDK (VMware) | vmdk
