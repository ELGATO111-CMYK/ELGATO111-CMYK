import math

# Meminta jari-jari lingkaran dari pengguna
jari_jari = float(input("Masukkan jari-jari lingkaran: "))

# Menghitung luas lingkaran
luas = math.pi * jari_jari ** 2

# Menampilkan hasil
print(f"Luas lingkaran dengan jari-jari {jari_jari} adalah {luas:.2f}")
