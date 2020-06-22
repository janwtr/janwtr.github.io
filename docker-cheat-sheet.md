# Docker Cheat Sheet

## Membuat tempat penyimpanan data dalam docker
- Docker memiliki dua opsi tempat untuk menyimpan file di mesin host, sehingga file tetap ada bahkan setelah kontainer berhenti: volumes, dan bind mounts
- Menjalankan container dengan __bind mounts__
  
  Source [https://docs.docker.com/storage/bind-mounts/](https://docs.docker.com/storage/bind-mounts/)
  ```
  $ docker run -d \
  -it \
  --name devtest \
  --mount type=bind,source="$(pwd)"/target,target=/app \
  nginx:latest
  ```
- Menjalankan container dengan __volumes__
  
  Source [https://docs.docker.com/storage/volumes/](https://docs.docker.com/storage/volumes/)
  ```
  $ docker run -d \
  --name devtest \
  --mount source=myvol2,target=/app \
  nginx:latest
  ```
## Build and Run docker
- Best practices for writing Dockerfiles
  
  Source [https://docs.docker.com/develop/develop-images/dockerfile_best-practices/](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
  
  Contoh `Dockfile`:
  ```
  FROM ubuntu:18.04
  COPY . /app
  RUN make /app
  CMD python /app/app.py
  ```
  
  - `FROM` membuat layer dari `ubuntu:18.04` Docker images
  - `COPY` menambahkan file dari direktori klien Docker saat ini.
  - `RUN` membangun aplikasi dengan make.
  - `CMD` menentukan perintah apa yang harus dijalankan dalam container.
  
-  Intruksi-instruksi Dockerfiles
  Source [https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#dockerfile-instructions](Best practices for writing Dockerfiles)
  
