# Run Ubuntu desktop in Windows 10
## In Windows:
- Install VcXsrv 
  
  Download: [https://sourceforge.net/projects/vcxsrv/](https://sourceforge.net/projects/vcxsrv/)
  
  Ikuti petunjukk instalasi

## In Ubuntu (wsl):
$ sudo apt-get update
$ sudo apt-get upgrade

$ sudo apt-get install xfce4
$ export DISPLAY=:0.0
$ startxfce4
