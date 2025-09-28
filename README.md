# MINPRO-DDP---2
Alya Aulia - Sistem Informasi

# FLOWCHART
<img width="2228" height="1335" alt="MINPRO-2" src="https://github.com/user-attachments/assets/8c512840-abb1-4fe1-b0bc-67ba61b0b034" />


# KODE PYTHON

print("halaman Awal")
print("silahkan Masuk Sebagai manajer/Karyawan")

pilihan = input("Input Pilihan (Karyawan/Manajer/Keluar): ")


if pilihan == "Manajer":
  print("Manajer")
  manajer = {
      "username": "Manajer",
      "password": "123"
  }

  kesempatan = 1
  while kesempatan > 0:
    username = input("Input Username: ")
    password = input("Input Password: ")

    if username == manajer["username"] and password == manajer["password"]:
      print("Login  Sebagai manajer Berhasil")
      print("Pilihan Opsi")
      print("1=Lihat Barang")
      print("2=Tambah Barang")
      print("3=Update Barang")
      print("4=Keluar")
      melihat = input("Pilih Opsi 1/2/3/4: ")
      if melihat == "1":
        print("Lihat Barang")
        barang = {
            "1.Tersedia": "Buku",
            "2.Tersedia": "Laptop"
        }
        x = barang.get("1.Tersedia"), barang.get("2.Tersedia")
        print(x)
      elif melihat == "2":
        print("Tambah Barang")
        barang = {
            "1.Tersedia": "Buku",
            "2.Tersedia": "Laptop"
        }
        barang["3.Tersedia"] = "Mouse"
        print(barang)
      elif melihat == "3":
        print("Update Barang")
        barang = {
            "1.Tersedia": "Buku",
            "2.Tersedia": "Laptop"
        }
        barang.update({"1.Tersedia": "Charger"})
        print(barang)
      elif melihat == "4":
        print("Keluar")
        
      else:
        print("Nomor salah")
      break




    else:
      kesempatan == 0
      print("Login Gagal, Kesempatan Habis")
      break
      

  
elif pilihan == "Karyawan":
    print("Karyawan")
    username = input("Input Username: ")
    password = input("Input Password: ")

    menu = input("Meminjam/Mengembalikan Barang?: ")
    if menu == "Meminjam":
        print("Silahkan Pilih Barang Yang Akan DiPinjam")

        barang = ["Buku", "Laptop"]
        print("barang")

        pinjam = input("Pilih(Buku/Laptop): ")
        if pinjam == "Buku":
            input("Input Tanggal Pemesanan: ")
            input("Input Tanggal Pengembalian: ")
            print("Peminjaman Barang Berhasil")
            barang.remove("Buku")
            print("Barang Pinjaman Yang Tersedia", barang)

        elif pinjam == "Laptop":
                input("Input Tanggal Pemesanan: ")
                input("Input Tanggal Pengembalian: ")
                print("Peminjaman Barang Berhasil")
                barang.remove("Laptop")
                print("Barang Pinjaman Yang Tersedia", barang)

        else:
            print("Barang Tidak Ada/Tidak Tersedia")

    elif menu == "Mengembalikan":
        print("Silahkan Pilih Barang Yang Akan DiKembalikan")

        barang = ["Buku", "Laptop"]
        print("barang")

        mengembalikan = input("Pilih (Buku/Laptop): ")
        if mengembalikan == "Buku":
            barang.remove("Buku")
            print("Barang Tersisa", barang)
            tanggal_1 = str(input("Input Tanggal Perjanjian Pengembalian: "))
            tanggal = str(input("Input Tanggal Pengembalian: "))
            if tanggal == tanggal_1:
                barang.append("Buku")
                print("Pengembalian Barang Tepat Waktu, Barang Tersedia", barang)
            else:
                print("Pengembalian Barang Tidak Tepat Waktu, Barang Tersedia", barang)

        elif mengembalikan == "Laptop":
            barang.remove("Laptop")
            print("Barang Tersisa", barang)
            tanggal_1 = str(input("Input Tanggal Perjanjian Pengembalian: "))
            tanggal = str(input("Input Tanggal Pengembalian: "))
            if tanggal == tanggal_1:
                barang.append("Laptop")
                print("Pengembalian Barang Tepat Waktu")
            else:
                print("Pengembalian Barang Tidak Tepat Waktu, Barang Tersedia", barang)

        else:
            print("Barang Tidak Termasuk")


elif pilihan == "Keluar":
    print("Keluar?")
    keluar = input("Ingin Keluar? (Ya/Tidak): ")
    if keluar == "Ya":
        print("Keluar dari halaman")
    else:
        print("Silahkan Pilih Karyawan/Manajer")

else:
    print("Pilihan salah/Tidak Ada")



# OUTPUT
KONDISI 1
<img width="1221" height="217" alt="kondisi 1" src="https://github.com/user-attachments/assets/fd5b281d-6bfa-4001-9202-a5c90716c84d" />
KONDISI 2
<img width="1265" height="274" alt="kondisi 2" src="https://github.com/user-attachments/assets/daa35395-8a3f-4639-a941-e403a2052d83" />
KONDISI 3
<img width="1247" height="273" alt="kondisi 3" src="https://github.com/user-attachments/assets/d6e77596-2cf3-4338-b3fc-fb6de3faee3b" />
KONDISI 4
<img width="1231" height="269" alt="kondisi 4" src="https://github.com/user-attachments/assets/cc179555-60bf-46ca-99ad-5e7e350ff876" />
KONDISI 5
<img width="1239" height="257" alt="kondisi 5" src="https://github.com/user-attachments/assets/736a20d3-5592-412b-84b4-1da126d1d7e5" />
KONDISI 6
<img width="1237" height="137" alt="kondisi 6" src="https://github.com/user-attachments/assets/2653aa06-7b4a-495a-b5e9-056de671476b" />
KONDISI 7
<img width="1249" height="263" alt="kondisi 7" src="https://github.com/user-attachments/assets/6b800168-b482-478a-b0ed-87c198bb5cde" />
KONDISI 8
<img width="1237" height="251" alt="kondisi 8" src="https://github.com/user-attachments/assets/227564f5-c15e-4abd-9dea-1f61e37fc0bb" />
KONDISI 9
<img width="1251" height="203" alt="kondisi 9" src="https://github.com/user-attachments/assets/fe67d636-732b-4e5c-a7d6-40d3c5cb93db" />
KONDISI 10
<img width="1239" height="255" alt="kondisi 10" src="https://github.com/user-attachments/assets/17d67b52-3b54-4adc-bee2-75d0446008d8" />
KONDISI 11
<img width="1241" height="253" alt="kondisi 11" src="https://github.com/user-attachments/assets/7b31b82a-c713-4a80-b27f-1c4c461b667d" />
KKONDISI 12
<img width="1257" height="207" alt="kondisi 12" src="https://github.com/user-attachments/assets/5c371147-7585-4de4-b835-ed924646b500" />




SELESAI :).....
