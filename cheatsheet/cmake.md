# CMake

## A Basic Starting Point
Buat file bernama `CMakeLists.txt`, misalnya berada di `\home\jan\Project\CMakeLists.txt` minimal isinya seperti ini:
```
cmake_minimum_required(VERSION 3.10)

# set the project name
project(Tutorial)

# add the executable
add_executable(Tutorial tutorial.cxx)
```
## Build and Test
1. Configure the project
    
    Untuk memisahkan direktori project dan file-file konfigurasi, buat direktori baru, misal `\home\jan\Project_build`, masuk ke direktori tersebut kemudian jalankan
    ```
    cmake \home\jan\Project
    ```
    atau
    ```
    cmake ..
    ```
    `CMakeLists.txt` tidak perlu dituliskan, cmake akan otomatis mencari file tersebut.
    di dalam `\home\jan\Project_build` akan dihasilkan file-file konfigurasi cmake yang siap untuk dilakukan Build System.
    
    Jika ingin menggulakukan _debuging_ gunakan:
    ```
    cmake -DCMAKE_BUILD_TYPE="Debug" ..
    ```
2. Call the build system
    
    Dari `\home\jan\Project_build`, jalankan
    ```
    cmake --build .
    ```
    artinya cmake akan melakukan _build_ berdasarkan file-file konfigurasi didirektori tersebut (ditunjukkan dengan tanda `.`).


## Tutorial Yang Berguna
Selanjutnya bisa mengikuti tutorial CMake berikut: https://cmake.org/cmake/help/v3.20/guide/tutorial/index.html#id1

