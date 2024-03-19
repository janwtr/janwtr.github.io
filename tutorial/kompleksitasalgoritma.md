## Contoh Algoritma Bubble Sort

Algoritma bubble sort adalah algoritma sorting yang sederhana dengan kompleksitas waktu O(n^2) dan kompleksitas memori O(n).

**Berikut adalah program bubble sort dalam bahasa Python:**

```python
def bubble_sort(arr):
    for i in range(len(arr) - 1):
        for j in range(len(arr) - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]

arr = [5, 1, 4, 2, 3]
bubble_sort(arr)
print(arr)
```

**Analisis Kompleksitas Waktu:**

* Loop for luar diulang sebanyak `len(arr) - 1` kali.
* Loop for dalam diulang sebanyak `len(arr) - i - 1` kali.
* Di dalam loop for dalam, terdapat operasi perbandingan `arr[j] > arr[j + 1]` dan operasi penukaran `arr[j], arr[j + 1] = arr[j + 1], arr[j]`.

Kompleksitas waktu total:

```
O(n) * O(n) = O(n^2)
```

**Analisis Kompleksitas Memori:**

* Program ini menggunakan array `arr` dengan panjang `n`.
* Selain itu, program ini menggunakan beberapa variabel lokal, seperti `i` dan `j`.

Kompleksitas memori total:

```
O(n) + O(1) = O(n)
```

**Kesimpulan:**

* Algoritma bubble sort memiliki kompleksitas waktu O(n^2) dan kompleksitas memori O(n).
* Algoritma ini tidak efisien untuk sorting array dengan ukuran yang besar.

**Contoh Algoritma Binary Search:**

Algoritma binary search adalah algoritma pencarian yang efisien dengan kompleksitas waktu O(log n) dan kompleksitas memori O(1).

**Berikut adalah program binary search dalam bahasa Python:**

```python
def binary_search(arr, target):
    left = 0
    right = len(arr) - 1

    while left <= right:
        mid = (left + right) // 2

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1

    return -1

arr = [1, 3, 5, 7, 9, 11, 13, 15]
target = 11
result = binary_search(arr, target)

if result != -1:
    print(f"Elemen ditemukan di indeks {result}")
else:
    print("Elemen tidak ditemukan")
```

**Analisis Kompleksitas Waktu:**

* Loop `while` diulang sebanyak `log n` kali.
* Di dalam loop `while`, terdapat operasi perbandingan `arr[mid] == target`, `arr[mid] < target`, dan `right = mid - 1`.

Kompleksitas waktu total:

```
O(log n)
```

**Analisis Kompleksitas Memori:**

* Program ini menggunakan array `arr` dengan panjang `n`.
* Selain itu, program ini menggunakan beberapa variabel lokal, seperti `left`, `right`, dan `mid`.

Kompleksitas memori total:

```
O(n) + O(1) = O(1)
```

**Kesimpulan:**

* Algoritma binary search memiliki kompleksitas waktu O(log n) dan kompleksitas memori O(1).
* Algoritma ini sangat efisien untuk pencarian data dalam array yang sudah diurutkan.

**Sumber informasi:**

* Algoritma Bubble Sort: [https://www.geeksforgeeks.org/bubble-sort/](https://www.geeksforgeeks.org/bubble-sort/)
* Analisis Kompleksitas Algoritma Bubble Sort: [http://repository.unika.ac.id/13294/5/12.60.0248%20Christina%20Thiveny%20Putrianti%20BAB%20IV.pdf](http://repository.unika.ac.id/13294/5/12.60.0248%20Christina%20Thiveny%20Putrianti%20BAB%20IV.pdf)
* Algoritma Binary Search: [[URL yang tidak valid dihapus]
