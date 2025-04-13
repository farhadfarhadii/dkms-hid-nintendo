# dkms-hid-nintendo

A Nintendo HID kernel module.

> [!NOTE]
>This repository contains changes from the patch comment [here](https://github.com/DanielOgorchock/linux/issues/40#issuecomment-2029009734).
>It allows the use of the Gulikit Kingkong 2 Pro Controller via Bluetooth (and possibly other third part controllers).
>

For any questions or bug reports, please refer to [hid_nintendo](https://github.com/DanielOgorchock/linux).


## Installation

Install it from source with:

HTTPS:

```sh
git clone https://github.com/farhadfarhadii/dkms-hid-nintendo
```

SSH:

```sh
git clone git@github.com:farhadfarhadii/dkms-hid-nintendo
```

```sh
cd dkms-hid-nintendo
git checkout third-party-support

sudo dkms add .
sudo dkms build nintendo -v 3.2
sudo dkms install nintendo -v 3.2
```

## Related projects

- [joycond](https://github.com/DanielOgorchock/joycond): A userspace daemon to
  combine joy-cons from the hid-nintendo kernel driver
- [joycond-cemuhook](https://github.com/joaorb64/joycond-cemuhook): Support for
  cemuhook's UDP protocol for joycond devices
