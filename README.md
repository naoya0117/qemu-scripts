# qemu-myenvironment
my qemu run scripts
## how to use
```
guest_os
├── iso
│   └── guest_os-image.iso
├── OVMF_VARS.fd (bios-data. if your distribution is Arch, run ```sudo pacman -S edk2-ovmf``` then ```cp /usr/share/ovmf/x64/OVMF_VARS.fd` ~/path/to/qemu-directory``
├── run.sh
├── tpm
│   └── (empty) (autogenerated by swtpm)
└── yourstorage-img(create with ```qemu-img create -f raw _image_file_ _size_```)
```

## example
```
Win11
├── iso
│   ├── virtio-win-0.1.229.iso
│   └── Win11_22H2_English_x64v2.iso
├── OVMF_VARS.fd
├── run.sh
├── tpm
│   └── tpm2-00.permall
└── windows11_img
```
```
Xubuntu
├── iso
│   └── xubuntu-22.04.3-desktop-amd64.iso
├── OVMF_VARS.fd
├── run.sh
├── tpm
│   └── tpm2-00.permall(auto-generate)
└── xubuntu_img

```
