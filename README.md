# RedHat_7_installation

### Download redhat 7 
* download RHEL 7.0 ISO Evaluation image from Red Hat Customer Portal.
* link is :https://access.redhat.com/products/red-hat-enterprise-linux#getstarted

### Create USB bootable

* for making bootable USB for installing redhat first install unitbootin by using following command
* `sudo apt-get install yum`
* insert usb into computer and Launch unitbootin
* select type USBDrive , browse your iso image file location and click ok
* or you can make bootable USB by using following command in terminal
* `# dd if=source of=target bs=byte size; sync`
* `# dd if=/home/downloads/rhel-server-7.0-x86_64-dvd.iso of=/dev/sdb1 bs=512M; sync`
  * source is location of your file
  * target is where you want to move
  * The bite Size is generally “some power of 2, and usually not less than 512 bytes i.e., 512, 1024, 2048, 4096, 8192, 16384, but can be any reasonable whole integer value.
  * sync option allows you to copy everything
* after completing plugout USB from computer 

### installation on virtual box

* open virtual box
* click on new
* enter the OS
