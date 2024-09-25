Berikut beberapa contoh program Python sederhana yang dapat dipahami dengan mudah oleh pemula:

1. Menghitung Luas Lingkaran

Program ini menghitung luas lingkaran berdasarkan jari-jari yang dimasukkan oleh pengguna.

import math

# Meminta jari-jari lingkaran dari pengguna
jari_jari = float(input("Masukkan jari-jari lingkaran: "))

# Menghitung luas lingkaran
luas = math.pi * jari_jari ** 2

# Menampilkan hasil
print(f"Luas lingkaran dengan jari-jari {jari_jari} adalah {luas:.2f}")

2. Program Tebak Angka

Program ini meminta pengguna untuk menebak angka yang dipilih secara acak oleh komputer.

import random

# Komputer memilih angka secara acak antara 1 hingga 10
angka_rahasia = random.randint(1, 10)

# Pengguna mencoba menebak
tebakan = int(input("Tebak angka antara 1 dan 10: "))

# Memeriksa apakah tebakan benar
if tebakan == angka_rahasia:
    print("Selamat, tebakan kamu benar!")
else:
    print(f"Maaf, tebakan kamu salah. Angka yang benar adalah {angka_rahasia}.")

3. Konversi Celcius ke Fahrenheit

Program ini mengonversi suhu dalam derajat Celcius ke Fahrenheit.

# Meminta input suhu dalam Celcius dari pengguna
celcius = float(input("Masukkan suhu dalam Celcius: "))

# Mengonversi Celcius ke Fahrenheit
fahrenheit = (celcius * 9/5) + 32

# Menampilkan hasil
print(f"{celcius} derajat Celcius adalah {fahrenheit} derajat Fahrenheit.")

4. Menghitung Faktorial

Program ini menghitung faktorial dari sebuah angka.

# Meminta input dari pengguna
angka = int(input("Masukkan angka: "))

# Inisialisasi hasil faktorial
faktorial = 1

# Menghitung faktorial
if angka < 0:
    print("Faktorial tidak terdefinisi untuk bilangan negatif.")
elif angka == 0:
    print("Faktorial dari 0 adalah 1.")
else:
    for i in range(1, angka + 1):
        faktorial *= i
    print(f"Faktorial dari {angka} adalah {faktorial}.")

5. Menghitung Jumlah Bilangan dalam Daftar

Program ini menghitung jumlah bilangan dalam sebuah daftar yang dimasukkan oleh pengguna.

# Meminta input dari pengguna
angka = input("Masukkan daftar angka yang dipisahkan dengan spasi: ")

# Memecah input menjadi daftar angka
daftar_angka = list(map(int, angka.split()))

# Menghitung jumlah bilangan dalam daftar
jumlah = sum(daftar_angka)

# Menampilkan hasil
print(f"Jumlah dari daftar angka tersebut adalah {jumlah}.")

6. Program Penghitung Kata

Program ini menghitung berapa banyak kata yang ada dalam sebuah kalimat.

# Meminta input kalimat dari pengguna
kalimat = input("Masukkan sebuah kalimat: ")

# Menghitung jumlah kata
jumlah_kata = len(kalimat.split())

# Menampilkan hasil
print(f"Jumlah kata dalam kalimat tersebut adalah {jumlah_kata}.")

7. Program Menampilkan Bilangan Prima

Program ini menampilkan semua bilangan prima hingga batas yang diberikan oleh pengguna.

# Fungsi untuk memeriksa apakah bilangan prima
def is_prima(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

# Meminta input batas dari pengguna
batas = int(input("Masukkan batas bilangan: "))

# Menampilkan bilangan prima hingga batas tersebut
print(f"Bilangan prima hingga {batas}:")
for i in range(2, batas + 1):
    if is_prima(i):
        print(i, end=" ")

8. Menghitung Bilangan Fibonacci

Program ini menghasilkan deret Fibonacci hingga angka tertentu.

# Meminta jumlah bilangan Fibonacci dari pengguna
n = int(input("Masukkan jumlah bilangan Fibonacci yang ingin ditampilkan: "))

# Inisialisasi dua bilangan pertama dalam deret Fibonacci
a, b = 0, 1

# Menampilkan deret Fibonacci
print("Deret Fibonacci:")
for _ in range(n):
    print(a, end=" ")
    a, b = b, a + b

9. Program Kalkulator BMI

Program ini menghitung Body Mass Index (BMI) berdasarkan tinggi dan berat badan pengguna.

# Meminta tinggi badan dan berat badan dari pengguna
tinggi = float(input("Masukkan tinggi badan Anda (dalam meter): "))
berat = float(input("Masukkan berat badan Anda (dalam kilogram): "))

# Menghitung BMI
bmi = berat / (tinggi ** 2)

# Menentukan kategori BMI
if bmi < 18.5:
    kategori = "Kurus"
elif 18.5 <= bmi < 24.9:
    kategori = "Normal"
elif 25 <= bmi < 29.9:
    kategori = "Berat Badan Berlebih"
else:
    kategori = "Obesitas"

# Menampilkan hasil
print(f"Indeks Massa Tubuh (BMI) Anda adalah {bmi:.2f}. Kategori: {kategori}.")

10. Membalik Urutan Teks

Program ini membalik urutan karakter dari teks yang dimasukkan pengguna.

# Meminta input dari pengguna
teks = input("Masukkan sebuah teks: ")

# Membalik teks
teks_terbalik = teks[::-1]

# Menampilkan hasil
print(f"Teks terbalik: {teks_terbalik}")

Dengan berbagai contoh ini, Anda bisa mulai memahami dan berlatih dengan dasar-dasar pemrograman Python. Setiap program menunjukkan berbagai konsep dasar seperti input, kondisi, perulangan, dan fungsi.

