# <h1 align="center">Laporan Praktikum Modul Dasar-Dasar Python untuk Sains Data</h1>
<p align="center">Afan Ramadhan</p>

## Dasar Teori

### 1. Variabel dan Tipe Data 

variabel adalah nama yang digunakan sebagai simbolis untuk menyimpan nilai data di dalam komputer[2]. Variabel digunakan untuk membantu programer memahami, mengingat, dan menggunakan informasi dalam progam. Setiap variabel memiliki nama, nilai, dan tipe data. Tipe data yang sering digunakan diantaranya string(str) yang berisi rangkaian karakter yang didefinisikan dengan tanda kutip(" "). Selain itu ada tipe data integer(int) yang berisi bilangan bulat. kemudian ada tipe data float yang memuat nilai desimal. Terakhir ada tipe data boolean yang berisi nilai benar atau salah.

### 2. Operator dan Logika

Operator adalah simbol yang digunakan untuk melakukan operasi pada suatu nilai atau variabel [1]. Didalam python terdapat beberapa operator yang dapat digunakan seperti operator aritmatika(+, -, *, /, %, //, **), operator perbandingan(<, >, =, ==, !=, <=, >=), dan operator logika(True, False). Selain operator ada juga logika yang merujuk pada proses penalaran dan pengambilan keputusan berdasarkan kondisi tertentu. Operator logika memungkinkan kita untuk menggabungkan beberapa pernyataan boolean dan menghasilkan hasil yang baru [1]. Dalam bahasa pemrograman, logika sangat penting yang biasa digunakan untuk pengkondisian untuk mengambil keputisan tertentu.

### 3. Fungsi

Fungsi adalah sebuah blok kode yang berisi sekumpulan pernyataan untuk melakukan suatu tindakan dan dapat dipanggil di bagian lain dari program [1]. Fungsi membantu memecah program menjadi bagian-bagian kecil yang lebih mudah dikelola. Ini membuat kode lebih terstruktur dan lebih mudah dipahami. fungsi akan sangat efektif jika digunakan untuk menulis code-code yang digunakan lebih dari 1 kali karena fungsi dapat dipanggil di lain progam sehingga mengurangi penulisan kode berulang yang dapat memakan waktu.

### 4. Pengulangan(loops)

Perulangan(looping) adalah cara untuk menjalankan sekelompok kode berulang kali berdasarkan kondisi tertentu. Dua jenis perulangan yang umum digunakan dalam banyak bahasa pemrograman adalah perulangan while dan perulangan for. Perulangan while merupakan perulangan akan terus mengeksekusi blok kode selama kondisi yang diberikan bernilai True. Ini berguna ketika jumlah iterasi tidak diketahui sebelumnya dan tergantung pada kondisi yang berubah selama proses. Sebaliknya untuk Perulangan for digunakan untuk mengiterasi elemen dari sebuah koleksi seperti daftar (list), tuple, string, atau rentang (range) angka. Ini sangat berguna ketika jumlah iterasi sudah diketahui.

### 5. Percabangan

Percabangan (branching) dalam pemrograman adalah cara untuk mengambil keputusan berdasarkan kondisi tertentu. Ini memungkinkan program untuk mengeksekusi bagian kode yang berbeda tergantung pada nilai kondisi [2]. Terdapat dua bentuk percabangan yang sering digunakan diantaranya if statment dan nested conditional (percabangan bersarang). If statement digunakan untuk mengevaluasi suatu kondisi. Jika kondisi tersebut bernilai True, maka blok kode di dalam pernyataan if akan dieksekusi. Jika kondisi tersebut bernilai False, blok kode tersebut akan dilewati. Sedangkan untuk Nested conditional merupakan if statemet yang berada di dalam if statement lain. Hal Ini memungkinkan kita untuk membuat keputusan yang lebih kompleks.

## Guided 

### 1. Variabel dan Tipe Data 

```python
x = 10 
y = 3.14 
z = "Data Science" 
user_age = 20 
pi_value = 3.14159 
course_name = "Python for Data Science" 
```

kode diatas merupakan kode yang bertujuan mendeklarasikan dan menginisialisasi 6 variabel dimana setiap variabel memiliki penamaan dan tipe data yang berbeda. Penamaan variabel tidak boleh mengguanakan sepasi, kebanyakan orang menggunakan under score untuk mengganti spasi.

### 2. Operator dan Logika

#### a. Operator Aritmatika

```python
a = 10 
b = 3 

# Penjumlahan 
print(a + b)   

# Pembagian 
print(a / b)   

# Pembagian bulat 
print(a // b)   

# Eksponensial 
print(a ** b)   
```

kode diatas berisi 2 variabel untuk dilakukan operasi aritmatika dasar(tambah, bagi, floor division, dan pangkat) dan menampilkannya ke layar dengan perintah print.

#### a. Operator Perbandingan

```python
print(a > b)  # Output: True 

print(a == b) # Output: False 
```

kode diatas merupakan penerapan operator perbandingan lebih besar(>) dan sama dengan(==) yang bertujuan untuk menentukan hubungan antara nilai a dan b serta menampilkan hasilnya menggunakan perintah print dam bentuk boolean. 

#### b. Operator Logika

```python
x = True 
y = False 
print(x and y) 
print(x or y) 
```

code diatas merupakan penerapan logika pada 2 variabel dan menampilkannya menggunakan perintah print. 

### 3. Fungsi

```python
# Definisi fungsi sederhana 

def greet(name): 
    return f"Hello, {name}!" 

# Memanggil fungsi 
print(greet("Agung"))
```

kode diatas mendemonstrasikan bagaimana mendefinisikan dan memanggil fungsi serta mengembalikan hasilnya berupa stirng yang berisi sapaan ke seseorang. 

### 4. Perulangan(loops)

#### a. For Loop

```python
fruits = ["apple", "banana", "cherry"] 
for fruit in fruits: 
    print(fruit)
```

kode ini menunjukan bagaimana cara melakukan iterasi melalui elemen dalam sebuah list dan mencetak setiap elemn yang ada.

#### b. While Loop

```python
counter = 0
while counter < 3: 
    print(counter) 
    counter += 1 
```

kode diatas menjelaskan bagaimana melakukan iterasi menggunakan while loop sampai kondisi dimana nilai dari variabel counter mencapai angka 3. sebelum mencapai angka 3 code akan mencetak setiap nilai dari variabel counter secara increment.

#### c. List Comprehension

```python
numbers = [1, 2, 3, 4, 5] 
doubled = [x * 2 for x in numbers] 
print(doubled) 
```

kode diatas merupakan modifikasi lain dari for loop dengan cara yang lebih efisien dimana dalam contoh ini setiap angka yang terdapat dalam numbers akan digandakan 2 menjadi variable doubled.

### 5. Percabangan

#### a. If, Elif, dan Else

```python
score = 85 
if score >= 90: 
    print("A") 
elif score >= 80: 
    print("B") 
else: 
    print("C") 
```

kode di atas merupakan contoh penerapan if statement untuk menentukan kategori huruf dari score yang didapat. Pada code tersebut jika score lebih besar sama dengan 90 atau 80 maka akan bernilai b dan jika score kurang 80 maka akan bernilai c. 

#### b. Nested Conditionals

```python
score = 85 
attendance = 90 
if score >= 80: 
    if attendance >= 85: 
        print("Lulus dengan nilai baik") 
    else: 
        print("Kehadiran kurang") 
else: 
    print("Tidak lulus")
```

kode ini menggunakan struktur kontrol bersarang untuk menentukan status kelulusan berdasarkan dua kondisi: nilai dan kehadiran. Ini menunjukkan cara untuk membuat keputusan yang lebih kompleks berdasarkan beberapa kondisi.

## Unguided 

### 1. Memecahkan Masalah Unik dengan Loop dan If-Else

```python
def prima(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

def segitiga_siku(data_list):
    idx = 0
    row = 1
    while idx < len(data_list):
        for i in range(row):
            if idx < len(data_list):
                print(data_list[idx], end=' ')
                idx += 1
        print()
        row += 1

def tampilkan(x):
    data_list = []
    for i in range(2, x + 1):
        if prima(i):
            data_list.append(i)
    segitiga_siku(data_list)

tampilkan(30) # limit
```
#### Output:
![1](https://github.com/user-attachments/assets/f4949c4e-e6d2-4fb2-8ff9-f63f47224f64)

Kode diatas merupakan implementasi untuk menemukan dan menampilkan bilangan prima dalam format segitiga siku-siku. Dalam kode tersebut terdapat 3 buah fungsi yaitu 'prima' yang digunakan untuk menentukan bilangan prima, 'segitiga_siku' yang berguna untuk menampilkan bilangan prima pada sebuah list dengan format segitiga siku-siku, dan 'tampilkan' untuk menyimpan bilangan prima ke dalam list.

### 2. Membuat Fungsi dengan Syarat Spesifik

```python
def list_ganjil(input1, input2):
    list_ganjil = []
    list1 = list(map(int, input1.split()))
    list2 = list(map(int, input2.split()))
    for i in [list1, list2]:
        for index, j in enumerate(i):
            if index % 2 != 0:
                list_ganjil.append(j)
    return list_ganjil
                
input1 = input("Masukan list 1 angka(pisahkan dengan spasi): ")
input2 = input("Masukan list 2 angka(pisahkan dengan spasi): ")
hasil = list_ganjil(input1, input2)
print(f"\nHasil: {hasil}")
```
#### Output:
![2](https://github.com/user-attachments/assets/0123ad77-68fc-48b7-a5b2-c30013e31d47)

code di atas berfungsi untuk mengambil dua daftar angka dari input pengguna, kemudian mengumpulkan angka yang berada di posisi ganjil dari kedua daftar tersebut dan mengembalikannya sebagai hasil. Kode ini mendefinisikan fungsi list_ganjil(input1, input2) yang mengumpulkan angka dari dua daftar input berdasarkan posisi ganjilnya

### 3. Exception Handling dalam Konteks Nyata

```python
saldo = 500000
pin = 112211
coba = 3

def struk(saldo, jumlah_transaksi, saldo_akhir):
    print(" Transaksi ".center(30, "="))
    print(f"saldo Awal :".ljust(20)+f"{saldo:,}".rjust(10))
    print(f"Saldo AKhir:".ljust(20)+f"{saldo_akhir:,}".rjust(10))
    print("-"*30)
    print(f"Jumlah Penarikan:".ljust(20)+f"{jumlah_transaksi:,}".rjust(10))
    print("="*30)
    print()
    
def transaksi(saldo, jumlah_transaksi):
    if jumlah_transaksi <= saldo and jumlah_transaksi > 0:
        saldo_akhir = saldo - jumlah_transaksi
        print("Uang Berhasil Ditarik!\n")
        struk(saldo, jumlah_transaksi, saldo_akhir)
        return saldo_akhir
    else:
        print("\nMasukan Jumlah Saldo Yang Tersedia!")
        return saldo

while coba > 0:
    input_pin = int(input("Masukan Pin: "))
    if input_pin == pin:
        print("Pin Benar")
        print(f"\nSaldo: {saldo:,}")
        jumlah_transaksi = int(input("Masukan Jumlah Uang Yang Ditarik: "))
        saldo = transaksi(saldo, jumlah_transaksi)
        break
    else:
        coba = coba - 1 
        print(f"pin salah! sisa percobaan: {coba}")
        if coba == 0:
            print("\nMaaf ATM anda terblokir!\nSilahkan coba lagi dalam 30 Tahun")
```
#### Output:
![3](https://github.com/user-attachments/assets/da8206a5-cecd-4632-9cb2-4639ffc826d6)

Kode ini mengimplementasikan sistem penarikan uang di ATM yang memerlukan autentikasi PIN. Pengguna diminta memasukkan PIN, dan jika benar, mereka dapat memasukkan jumlah uang yang ingin ditarik. Fungsi transaksi memeriksa apakah jumlah penarikan valid dan memperbarui saldo, lalu mencetak struk transaksi. Jika PIN salah, jumlah percobaan berkurang, dan setelah tiga kali percobaan, sistem menginformasikan bahwa ATM terblokir.

### 4. Studi Kasus Pengelolaan Data

```python
import pandas as pd
import numpy as np

data_dict = {}
df = pd.read_csv("siswa_nilai (1).csv")

for i, row in df.iterrows():
    key = row['Nama Siswa']
    value = row['Nilai']
    data_dict[key] = value

nilai = np.array(list(data_dict.values()))
mean = np.mean(nilai)
min = np.min(nilai)
max = np.max(nilai)

print(f"Nilai Rata-rata: {mean}")
print(f"Nilai Minimum  : {min}")
print(f"Nilai Maksimum : {max}")
```
#### Output:
![4](https://github.com/user-attachments/assets/a1fd5f93-11e6-4bad-8940-0f6a4e8a95b7)

kode diatas bertujuan membaca file csv() dengan mengimpor pustaka pandas dan numpy, kemudian membaca data dari file CSV ke dalam DataFrame menggunakan pd.read_csv(). Selanjutnya, kode mengiterasi setiap baris DataFrame, mengambil nama siswa dan nilai, lalu menyimpannya ke dalam dictionary data_dict. Setelah itu, nilai-nilai diambil sebagai array menggunakan np.array() untuk menghitung rata-rata, nilai minimum, dan maksimum dengan menggunakan fungsi np.mean(), np.min(), dan np.max(). Terakhir, kode mencetak hasil perhitungan nilai rata-rata, minimum, dan maksimum.

### 5. Kombinasi Logika dan Kreativitas

```python
import random 

print(" Game Tebak Angka ".center(30, "="))

def tebak_angka():
    angka_random = random.randint(1, 100)
    coba = 5
    while coba > 0:
        tebak = int(input("Masukan Angka: "))
        if tebak == angka_random:
            print(f"Selamat Anda Berhasil Menebak Angka Yang Benar: {angka_random}")
            break
        else:
            coba = coba - 1
            if tebak < angka_random:
                print("Angka yang ditebak lebih besar")
            else:
                print("Angka yang ditebak lebih kecil")
            print(f"Percobaan tersisa: {coba}\n")
            
        if coba == 0:
            print(f"Kamu Gagal!\njawaban yang benar: {angka_random}")

tebak_angka()
```
#### Output: 
![5](https://github.com/user-attachments/assets/a5bdda2e-0694-48d5-81f9-5aa8618cf88c)

kode diatas merupakan mplementasi sederhana dari permainan tebak angka, di mana pemain diminta untuk menebak angka yang dihasilkan secara acak. Berikut adalah penjelasan singkat dalam empat kalimat. Angka acak dihasilkan dengan bantuan library random yang akan menghasilkan angkan acak antara 1-100.

### 6. Rekursi yang Tidak Biasa

```python
def rekursif(n):
    list_hasil = []
    def faktorial(i):
        if i == 0 or i == 1:
            return 1
        else:
            return i * faktorial(i - 1)
    for i in range(n + 1):
        list_hasil.append(faktorial(i))
    
    return list_hasil

input_n = int(input("Masukan n: "))
print(f"\nHasil: {rekursif(input_n)}")
```
Output:
![6](https://github.com/user-attachments/assets/ad7ecf32-33bb-4571-8517-c75ae40521c7)

code diatas merupakan code yang bertujuan untuk menghitung dan menampilkan faktorial dari semua angka mulai dari 0 hingga n, di mana n ditentukan oleh input pengguna. Dengan menggunakan pendekatan rekursif, kode ini memperlihatkan cara untuk menghitung faktorial sebuah operasi matematika yang mengalikan angka dengan semua angka bulat positif di bawahnya hingga 1. Hasilnya disimpan dalam sebuah daftar dan kemudian dicetak, memberikan pengguna pemahaman tentang bagaimana faktorial berkembang seiring dengan bertambahnya nilai n


### 7. Pemrograman dengan Algoritma Greedy

``` python
print(" Minimum Coin Change ".center(30, "="))
pecahan_koin = [25, 10, 5, 1]
hasil = []
koin = int(input("Masukan Koin: "))

for i in pecahan_koin:
    while koin >= i:
        koin -= i
        hasil.append(i)

print(f"Minimal pecahan koin yang dibutuhkan adalah {hasil}, {len(hasil)} koin")
```
Output:
![7](https://github.com/user-attachments/assets/beaa747a-7116-4c9d-952e-b51975456615)

Kode diatas digunakan untuk menghitung kombinasi minimal koin yang dibutuhkan untuk mencapai jumlah tertentu yang dimasukkan oleh pengguna. Denominasi koin yang digunakan terdiri dari 25, 10, 5, dan 1. Melalui loop, kode mengurangi jumlah koin yang dimasukkan dengan pecahan koin yang sesuai dan mencatat koin yang digunakan dalam daftar. Setelah selesai, kode mencetak daftar koin yang diperlukan beserta jumlah total koin yang digunakan.

### 8. Kombinasi String dan Manipulasi List

```python
kalimat = str(input("Masukan Kalimat: "))
kata = kalimat.split()
reverse = []

for i in range(len(kata)):
    kata_reverse = ""
    for huruf in reversed(kata[i]):
        kata_reverse = kata_reverse + huruf
    reverse.append(kata_reverse)

print(f"\nhasil: {reverse}")
```
Output:
![8](https://github.com/user-attachments/assets/6a11e1aa-9128-4233-96c9-72d320d60892)

Kode ini membalikkan setiap kata dalam kalimat yang dimasukkan oleh pengguna. Setelah menerima input, kalimat dibagi menjadi daftar kata menggunakan metode split(). Kemudian, setiap kata diiterasi dan dibalik menggunakan fungsi reversed(), hasilnya disimpan dalam daftar baru. Akhirnya, kode mencetak daftar kata yang telah dibalik sebagai output.

### 9. Konsep Class dan Object-Oriented Programming

```python
import datetime

class Buku:
    def __init__(self ,judul, penulis, tahun_terbit):
        self.judul = judul
        self.penulis = penulis
        self.tahun_terbit = tahun_terbit

    def info(self):
        print(" Informasi Buku ".center(30, "="))
        print(f"Judul\t\t: {self.judul}")
        print(f"Penerbit\t: {self.penulis}")
        print(f"Tahun Terbit\t: {self.tahun_terbit}")
        print()
    
    def umur_buku(self):
        print(" Informasi Umur Buku ".center(30, "="))
        umur = datetime.datetime.now().year - self.tahun_terbit
        print(f'Usia buku "{self.judul}" adalah {umur} tahun')
        print()
        
buku1 = Buku("Hafalan Solat Delisa", "Tere Liye", 2005)
buku2 = Buku("Tentang Kamu", "Tere Liye", 2016)
buku3 = Buku("Janji", "Tere Liye", 2021)

for buku in [buku1, buku2, buku3]:
    buku.info()
    buku.umur_buku()
```
Output:
![9](https://github.com/user-attachments/assets/a243ca22-bbba-40e4-b146-f4d2ec85a756)

Kode ini mendefinisikan kelas Buku yang menyimpan informasi tentang judul, penulis, dan tahun terbit buku. Metode info() mencetak detail buku, sedangkan metode umur_buku() menghitung dan menampilkan usia buku berdasarkan tahun terbit. Tiga objek buku dibuat dengan informasi yang berbeda, dan kemudian informasi serta umur masing-masing buku ditampilkan menggunakan loop. 

### 10. Algoritma dengan Persyaratan Logika Khusus

```python
import numpy as np

def binary_search(arr, target):
    arr = np.sort(arr)
    low = 0
    high = len(arr) - 1
    
    while low <= high:
        mid = (low + high) // 2
        
        if arr[mid] == target: 
            if arr[mid] % 2 == 0:
                return print(f"Nilai {target} ditemukan pada indeks ke-{mid}!")
            else:
                break
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
            
    return print(f"Nilai {target} tidak bisa ditemukan!")

arr = np.array([1,7, 5, 8, 9, 6, 5])
target = int(input("Masukan angka yang dicari: "))
binary_search(arr, target)
```
Output:
![10](https://github.com/user-attachments/assets/0de0aee2-9d49-42db-92be-fd9f25ee2bbe)

Kode ini mengimplementasikan pencarian biner untuk menemukan nilai target dalam array yang tidak terurut. Array diurutkan terlebih dahulu menggunakan np.sort(), kemudian algoritma pencarian biner digunakan untuk mencari nilai target. Jika nilai ditemukan dan genap, indeksnya dicetak; jika tidak, pencarian dihentikan tanpa output tambahan. Jika nilai target tidak ditemukan dalam array, kode mencetak pesan bahwa nilai tersebut tidak dapat ditemukan.

## Kesimpulan
Dalam Python, variabel dan tipe data adalah fundamental untuk menyimpan dan mengelola informasi. Variabel memungkinkan programer untuk memberi nama pada data dan mengaksesnya dengan cara yang lebih intuitif. Sementara itu berbagai tipe data seperti integer, float, string, dan boolean memungkinkan pemrograman yang lebih fleksibel dan beragam sesuai dengan kebutuhan aplikasi yang dikembangkan. Dengan kombinasi ini, programer dapat menyimpan informasi dan mengolahnya dengan cara yang efisien.

Selain itu, konsep seperti fungsi, percabangan, perulangan, operator, dan logika meningkatkan kemampuan pemrograman dengan memberikan struktur dan kontrol alur eksekusi. Fungsi memungkinkan programer untuk menulis kode yang modular dan dapat digunakan kembali. Sementara itu, percabangan dan perulangan memudahkan programer dalam pengambilan keputusan dan pengulangan proses secara efisien. Operator dan logika mendukung pengolahan data dan evaluasi kondisi yang sangat penting dalam pembuatan algoritma. Secara keseluruhan, elemen-elemen ini bekerja sama untuk menciptakan kode yang lebih terstruktur, mudah dibaca, dan efektif dalam menyelesaikan masalah kompleks.

## Referensi
[1] A. Kadir, "Dasar Pemrograman Python 3". Yogyakarta: Andi Publisher, 2018.