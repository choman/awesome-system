# awesome-system


## Install (lvm encrypt setup)






## ZFS Setup (zpool encrypt setup)
- ```sudo zpool create data /dev/nvme0n1 /dev/nvme1n1 /dev/nvme2n1 /dev/nvme3n1``` # (no encryption yet)

## ZFS Testing
- ```sudo hdparm -tT /dev/nvme0n1``` (device)
- `sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=20k; sudo sync`
- ```sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read```


## Virtual Machine Testing
- ubuntu 23.04b
  - 11:31m
- ubuntu 23.04b ssd
  - 


 

## Notes
```

    1  sudo apt update; sudo apt dist-upgrade -y
    2  sudo apt install zfsutils-linux
    3  sudo reboot 
    4  zfs 
    5  zpool 
    6  lsblk
    7  sudo zpool create data /dev/nvme1 /dev/nvme2 /dev/nvme3 /dev/nvme4
    8  fdisk -l
    9  sudo zpool create data /dev/nvme0n1 /dev/nvme1n1 /dev/nvme2n1 /dev/nvme3m1
   10  sudo zpool create data /dev/nvme0n1 /dev/nvme1n1 /dev/nvme2n1 /dev/nvme3n1
   11  zpool list
   12  cd /data/
   13  ls
   14  sudo hdparm -tT /data
   15  lsblk
   16  zfs list
   17  sudo hdparm -tT /dev/nvme0n1
   18  sync; dd if=/dev/zero of=tempfile bs=1M count=1024; sync
   19  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=1024; sudo sync
   20  lsblk
   21  lsblk -o NAME,FSTYPE,LABEL,MOUNTPOINT,SIZE,MODEL
   22  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=10k; sudo sync
   23  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=2\0k; sudo sync
   24  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=20k; sudo sync
   25  sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read
   26  sudo apt instal fio
   27  sudo apt install fio
   28  sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read
   29  man fio
   30  lspci
   31  lspci |grep -i dell
   32  sudo poweroff
   33  zpool list
   34  sudo zpool create data /dev/nvme0n1 /dev/nvme1n1 /dev/nvme2n1 /dev/nvme3n1
   35  zpool list
   36  cd /data
   37  sudo hdparm -tT /data
   38  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=1024; sudo sync
   39  sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read
   40  sudo hdparm -tT /dev/nvme0n1
   41  cd Downloads/
   42  ls
   43  tar tf ventoy-1.0.90-linux.tar.gz 
   44  ls
   45  tar xpf ventoy-1.0.90-linux.tar.gz 
   46  cd ventoy-1.0.90/
   47  ls
   48  ./VentoyGUI.x86_64
   49  cd
   50  cd /media/choman/Ventoy/
   51  ls
   52  mkdir ubuntu
   53  mv *iso ubuntu
   54  mkdir samsung
   55  mv ~/Downloads/Samsung_SSD_980_PRO_5B2QGXA7.iso samsung/
   56  cd
   57  history 
   58  sudo reboot 
   59  history 
   60  sudo poweroff
   61  zpool list
   62  sudo hdparm -tT /dev/nvme0n1
   63  cd /data/
   64  ls
   65  sync; dd if=/dev/zero of=tempfile bs=1M count=1024; sync
   66  sudo sync; sudo dd if=/dev/zero of=tempfile bs=1M count=1024; sudo sync
   67  sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read
   68  time sudo fio --filename=/data/test.bin --direct=1 --rw=read --ioengine=libaio --bs=2m --iodepth=64 --size=10G --numjobs=1 --runtime=60 --time_base=1 --group_reporting --name=test-seq-read
   69  du -sh (
   70  du -sh *
   71  history 
   72  lsblk
   73  zpool list
   74  zfs list
   75  ls -al
   76  df -h /
   77  df -h /home
   78  ls -la
   79  sudo apt install git
   80  ls
   81  l;s -la
   82  ls -la
   83  ssh-keygen 
   84  ssh-keygen  --help
   85  ssh-keygen  -t ed25519
   86  cat ~/.ssh/id_ed25519.pub 
   87  mkdir repos
   88  cd repos/
   89  ls
   90  git clone git@github.com:choman/awesome-system.git
   91  ls
   92  cd awesome-system/
   93  ls
   94  echo "# awesome-system" >> README.md
   95  git init
   96  git add README.md
   97  git commit -m "first commit"
   98  git branch -M main
   99  git remote add origin git@github.com:choman/awesome-system.git
  100  git push -u origin main
  101  ls
  102  git add README.md ; git commit -m "initi"; git push
  103  git config --global user.email choman@gmail.com
  104  git config --global user.name "Chad Homan"
  105  git push -u origin main
  106  git add README.md ; git commit -m "initi"; git push
  107  ls
  108  ls -la
  109  history 
  110  history  >> README.md 
```
