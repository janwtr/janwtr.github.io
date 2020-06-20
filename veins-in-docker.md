# Intalasi Veins 5.0 di Docker
## Persiapan
1. Komputer dengan Sistem Operasi Windows 10 dan terhubung dengan Internet
1. Docker desktop [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)
1. x11docker [https://github.com/mviereck/x11docker](https://github.com/mviereck/x11docker)
1. Veins 5.0 [https://veins.car2x.org/download/](https://veins.car2x.org/download/)
1. OMNeT++ 5.6.2 [https://omnetpp.org/download/](https://omnetpp.org/download/) (unduh yang versi docker)
1. SUMO 1.2.0 [https://sourceforge.net/projects/sumo/files/sumo/](https://sourceforge.net/projects/sumo/files/sumo/)
## Langakah
### Pasang Docker Desktop
1. Dokumentasi ada di [https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/), setelah diunduh tinggal klik instal dan ikuti petujuknya.
1. Pastikan docker sudah "running"

### Install VcXsrv Windows X Server
1. Jalankan instalasi seperti biasa sampai pada tampilan __Extra Settings__
1. Ketika sampai pada __Extra Settings__ beri centang apda __Disable Access control__, lanjuttkan dengan klik __Next__ sampai finish

### Pasang OMNeT++
1. Jalankan command promt dan ketikkan perintah
    ```cmd
    > docker pull omnetpp/omnetpp-gui:u18.04-5.6.2
    ```
1. Melihat docker images yang sudah di-pull tadi
    ```
    > docker images
    ```
1. Jalankan container OMNet dengan mode interaktif (menampilkan bash shell), sekaligus meberi nama container sebagai "veins"
    ```
    > docker run --rm -it -e DISPLAY=192.168.1.8:0.0 omnetpp/omnetpp-gui:u18.04-5.6.2
    ```
    1. Jika ingin menggunakan container lagi yang sama
        ```
        > docker run -it -e DISPLAY=192.168.1.8:0.0 --name veins omnetpp/omnetpp-gui:u18.04-5.6.2
        ```
    1. Menjalankan container lagi
        ```
        > docker start -i veins
        ```    
    
1. Selanjutnya akan masuk kedalam container "veins" dengan tampilan sebagai berikut
    ```
    omnetpp-gui-5.6.2:/root/models$
    ```
1. Menjalankan OMNet++
    ```
    $ omnetpp
    ```
    Maka akan menampilkan GUI OMNet++
    

### 


