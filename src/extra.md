sudo rmmod hid_nintendo
sudo dkms remove nintendo/3.2
sudo dkms add .
sudo build nintendo -v 3.2
sudo install nintendo -v 3.2
lsmod | grep hid_nintendo
