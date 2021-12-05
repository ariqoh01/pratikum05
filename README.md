# pratikum05
### A. Program

![img 1](Ss/01.PNG)

![img 2](Ss/02.PNG)

![img 3](Ss/03.PNG)

![img 4](Ss/04.PNG)

### C. Penjelasan

1. Membuat dictionary kosong yang nantinya akan diinput dengan data.
	```python
	data={}
	```

2. Membuat perulangan dengan _while_ dan terdapat pilihan menu untuk menjalankan program.
	```python
	while True:
    print()
    a=input("[(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar] :")
    print()
	```
3. Menambahkan data nim, nama, nilai tugas, uts, dan uas. Data yang diinputkan akan masuk ke dalam dictionary **data** dengan **nim** sebagai keys sedangkan nama, tugas, uts dan uas sebagai **values**.
	```python
	if a=="t" or a=="T":
        print("TAMBAH DATA")
        print("-----------")
        nim=int(input("NIM\t: "))
        nama=input("Nama\t: ")
        tugas=int(input("Tugas\t: ")) 
        uts=int(input("UTS\t: "))
        uas=int(input("UAS\t: "))
        akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)
        data[nim]=nama, tugas, uts, uas, akhir
	```
4. Menampilkan atau melihat data. Jika sebelumnya belum menginput data, maka tampilannya akan "Tidak ada data". Apabila sudah menginput data, maka data yang telah diinput tadi akan ditampilkan.
	```python
	elif a=="l" or a=="L":
        if data.items():
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            for item in data.items(): 
                print("| {0:>10} | {1:>10} | {2:>6} | {3:>6} | {4:>6} |   {5:>12}  |".format(nim, nama, tugas, uts, uas, akhir))
                print(72*"=")
            print()
        else:
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            print("|                             TIDAK ADA DATA                           |")
            print(72*"=")
            print()
	```
5. Apabila ingin mengubah data, maka anda akan diminta untuk menginputkan **nim** terlebih dahulu. Setelah itu input data yang ingin diubah.
	```python
	 elif a=="u" or a=="U":
        print("UBAH DATA")
        print("---------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            tugas=int(input("Tugas\t: ")) 
            uts=int(input("UTS\t: "))
            uas=int(input("UAS\t: "))
            akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)
	```
6. Jika ingin menghapus data, anda akan diminta untuk menginput **nim**. Lalu data yang telah diinput diawal tadi akan dihapus beserta valuesnya (nama, nilai tugas, nilai uts dan nilai uas).
	```python
	elif a=="h" or a=="H":
        print("HAPUS DATA")
        print("----------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            del data[nim]
	```
7. Apabila ingin mencari data, anda akan diminta untuk menginput **nim** kemudian data yang anda cari akan muncul berdasarkan nim yang diinput tadi.
	```python
	elif a=="c" or a=="C":
        print("CARI DATA")
        print("---------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            print("| {0:>10} | {1:>10} | {2:>6} | {3:>6} | {4:>6} |   {5:>12}  |".format(nim, nama, tugas, uts, uas, akhir))
            print(72*"=")
            print()
	```
8. Jika data sudah selesai diinput, pilih menu **'k'/'K'** maka program akan terhenti.
	```python
	elif a=="k" or a=="K":
         break
	```
### D. Output

![img 5](Ss/05.PNG)

![img 6](Ss/06.PNG)

![img 7](Ss/07.PNG)

![img 8](Ss/08.PNG)

![img 9](Ss/09.PNG)

![img 10](Ss/10.PNG)

![img 11](Ss/11.PNG)

![img 12](Ss/12.PNG)

![img 13](Ss/13.PNG)

![img 14](Ss/flowchart.jpg)

### Sekian Terimakasih
