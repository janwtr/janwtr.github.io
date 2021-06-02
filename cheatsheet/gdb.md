# GDB
GDB adalah _debuger_ untuk C dan C++.

## Compiling
Untuk dapat melakukan  _debuging_ gunakan `-g` flag saat melakukan kompilasi
    
```
gcc -g -o program program.c
```

Jika menggunakan CMake, gunkan tipe `Debug`

```
cmake -DCMAKE_BUILD_TYPE="Debug" ..
```

## Menjalankan GDB
```
gdb <program>
```
akan muncul promp
```
(gdb)
```
Untuk keluar ketikkan perintah `quit`

## Perintah-perintah dalam GDB
Command | Description
-------:|------------
`help` | Melihat dokumentasi GDB
`run` | Mulai menjalankan program dalam mode debug
`break` | Menentukan posisi _brakpoint_. `break <function>` atau `break <nomor baris>` atau `break <namafile:nomorbaris>`.
`delete` | menghapus semua _breakpoint_. `delete <nomor>` hanya menghapus _breakpoint_ pada nmor baris tertentu.
`clear` | `clear <function>` hanya kan menghapus  _breakpoint_ pada fungsi tertentu.
`continue`| Melanjutkan program untuk jalan kembali
`step`| Menjalankan program satu langkah kemudian berhenti lagi
`next`| seperti step hanyasaja menjalankan satu langkah fungsi sampai selesai
`until`|sama seperti step namun akan berhenti sampiai selesai dari sebuah loop
`list`| `list <nomorbaris>` akan menampilkan kode program disekitar `nomorbaris` tersebut. Jika tanpa argumen akan menampilan kode disekitar posisi berhenti.
`print`| `print <expression>` akan menampilkan nilai dari `expression` yg diinginkan, misalnya suatu variable tertentu.
