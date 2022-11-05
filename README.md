# ddrescue-bootable

First you need to install ddrescue and install the image file of distro

```bash
apt install gddrescue
```
Now check the location of pendrive
```bash
sudo fdisk -l
```
the location of the pendrive would probably at the end:
![image](https://user-images.githubusercontent.com/95766110/200100691-d937cf33-56b4-40d9-9c9f-0c2c1d3a7d3f.png)

In this case mine is /dev/sdb

Now go to the dir where the iso file is downloaded and run the following command:
```bash
sudo ddrescue <name of the iso file that you downloaded> <location of the pendrive> --force -D
```
In this case it is:
```bash
sudo ddrescue ubuntu-16.04.7-server-amd64.iso /dev/sdb --force -D
```
Now the process will start.
Wait for few minutes until the process is finished.
