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
Dokumentasi ada di [https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/), setelah diunduh tinggal klik instal dan ikuti petujuknya.

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
    > docker run --interactive --tty --name veins omnetpp/omnetpp-gui:u18.04-5.6.2 bash
    ```
1. Selanjutnya akan masuk kedalam container "veins" dengan tampilan sebagai berikut
    ```
    omnetpp-gui-5.6.2:/root/models$
    ```
1. Update ubuntu terlebih dulu (omnetpp-gui images berbasis ubuntu)
    ```
    $ apt update
    ```
1. Install xfce4 untuk Desktop Environment di linux
    ```
    $ apt install xfce4
    ```    
1. Tambahkan "export DISPLAY=:0.0" pada .bashrc
    ```
    $ cd ~
    $ cat >>.bashrc
    export DISPLAY=:0.0
    ```
    tekan __Ctrl+D__ untuk selesai
    

1. Menjalankan lagi container yang telah dibuat
    ```
    docker start -i veins
    ```
## Tidak berhasil
