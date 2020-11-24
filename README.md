**Nama : Ainul Yaqin**
**NIM : 312010423**
**Kelas : TI.20.A.1**


# **Program Data Mahasiswa**

# Pertemuan 9 - Praktikum Modul 4 <br>
Pada praktikum kali ini saya akan membuat program sederhana untuk menginput data kedalam list. <br>
![gambar](Gambar/gambar1.png) <br>
![gambar](Gambar/gambar2.png) <br>
![gambar](Gambar/gambar3.png) <br>

Berikut Inputannya :

`nilai = []` <br>
`ulang = True` <br>

`while ulang:` <br>
`    nama = input("Masukkan Nama: ")` <br>
`    nim = input("Masukkan NIM: ")` <br>
`    tugas = int(input("Masukkan Nilai Tugas: "))` <br>
`    uts = int(input("Masukkan Nilai UTS: "))` <br>
`    uas = int(input("Masukkan Nilai UAS: "))` <br>
`    akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)`

`    nilai.append([nama, nim, tugas, uts, uas, int(akhir)])` <br>
`    if (input("Tambah data (y/t)?") == 't'):` <br>
`        ulang = False`

`print("\n                      Daftar Nilai Mahasiswa")` <br>
`print("==================================================================")` <br>
`print("|No. |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")` <br>
`print("==================================================================")` <br>
`i = 0` <br>
`for item in nilai:` <br>
`    i += 1` <br>
`    print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"` <br>
`          .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))` <br>
`print("==================================================================")`

`#Program Data Mahasiswa`

`Program praktikum`

# Penjelasan : <br>
* Pertama kita membuat Variabel list kosong. <br>
`nilai = []` <br>
`ulang = True` <br>
Variabel `ulang = True` digunakan untuk mengontrol perulangan. <br>
* Lalu kita membuat kondisi perulangan dan statement yang akan dijalankan ketika perulangan terjadi. <br>
`while ulang:` <br>
`    nama = input("Masukkan Nama: ")` <br>
`    nim = input("Masukkan NIM: ")` <br>
`    tugas = int(input("Masukkan Nilai Tugas: "))` <br>
`    uts = int(input("Masukkan Nilai UTS: "))` <br>
`    uas = int(input("Masukkan Nilai UTS: "))` <br>
`    akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35 100)`

`    nilai.append([nama, nim, tugas, uts, uas, int(akhir)])` <br>
Dari statement diatas, kita akan diminta untuk menginput nama, nim, nilai tugas, nilai uts, dan nilai uas, lalu system akan menjumlahkan nilai-nilai tersebut dan menghasilkan nilai akhir. Setelah menginput berbagai data atau item, inputan item tersebut akan masuk ke dalam list 'nilai' <br>
*  Setelah membuat perulangan, kita membuat statement untuk menghentikan atau keluar dari perulangan yang terjadi. <br>
`if (input("Tambah data (y/t)?") == 't'):` <br>
`        ulang = False` <br>
Untuk keluar dari perulangan kita hanya perlu menginputkan 't' apabila diminta pada saat program dijalankan. 't' akan membuat variable `ulang = True` menjadi `ulang = False` yang mana akan menghentikan perulangan yang terjadi. <br>
* Dan Yang terakhir kita akan mencetak hasil dari program yang telah di buat. <br>
`print("\n                      Daftar Nilai Mahasiswa")` <br>
`print("==================================================================")` <br>
`print("|No. |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")` <br>
`print("==================================================================")` <br>
`i = 0` <br>
`for item in nilai:` <br>
`    i += 1` <br>
`    print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"` <br>
`          .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))` <br>
`print("==================================================================")`

**Berikut ini Hasinya:**

![gambar](Gambar/Hasil1.png) <br>

# Pertemuan 9 Modul 5 <br>
Pada Pertemuan 9 Modul 5 dosen memberikan saya tugas untuk membuat program sederhana yang akan menampilkan daftar nilai mahasiswa. berikut soal yang dosen berikan: <br>
![gambar](Gamabar/gambar4.png) <br>
# Penjelasan : <br>
* Penggunaan if c.lower() if c.lower() fungsinya apabila user menginputkan dengan huruf besar, maka otomatis akan menjadi huruf kecil sehingga kondisi yang diinginkan tercapai. contoh: `if c.lower() == 'q'` <br>
* Penggunaan while True while True berfungsi untuk mendeteksi jika format yang diinputkan bukan berupa type maka akan muncul eror <br>
* Penggunaan else Fungsi else ialah jika tidak eror dan type yang dimasukan sesuai maka proses while True. <br>
* Pengunaan valueError Fungsinya apabila diinputkan bukan berupa type maka hasilnya error (valueError) <br>
berikut source codenya: <br>
`                    while (True):` <br>
`                        nama = input(" Nama : ")` <br>
`                        if nama == '':` <br>
`                            P(' Masukan dengan Nama Dengan Benar')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            nim  = int(input(" NIM  : "))` <br>
`                            if nim == '':` <br>
`                                P(' Masukan Nim dengan Angka')` <br>
`                        except ValueError:` <br>
`                            P(' Masukan Nim dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            tugas  = int(input(" TUGAS  : "))` <br>
`                            if tugas == '':` <br>
`                                P(' Masukan TUGAS dengan Angka')` <br>
`                        except ValueError:
`                            P(' Masukan TUGAS dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
* Pengunaan round dan float round digunakan untuk menentukan banyaknya angka di belakang koma, sedangkan float digunakan untuk mengubah bilangan menjadi float(desimal) <br>
Berukut Source codenya: <br>
`akhir = round((float(tugas) * 0.3)+(float(uts) * 0.35)+(float(uas) * 0.35),2)` <br>
`        i.write('\nNama : '+nama+'|Nim : '+str(nim)+'|Tugas : '+str(tugas)+'|UTS : '+str(uts)+'|UAS : '+str(uas)+"|Akhir : "+str(akhir)+'\n')` <br>
`        i.close()` <br>
* Penggunaan Database.txt Berguna untuk menyimpan data dari inputan. <br>
![gambar](Gambar/gambar5.png)

`#Membuat Program Sederhana Menampilkan Daftar Nilai Mahasiswa` <br>
`#Ainul Yaqin` <br>
`#TI.20.A.1`

`P = print` <br>
`while True:` <br>
`    P("")` <br>
`    P("")` <br>
`    c = input("L)ihat, T)ambah, U)bah, H)apus, C)ari, K)eluar: ")` <br>
`    if c.lower() == 'q':` <br>
`        break` <br>
`    elif c.lower() == 'l':` <br>
`        i = open('database.txt','r').read().splitlines()` <br>
`        P(" ╔═════════════════════════════════════════════════════════════════════╗")` <br>
`        P(" ╠════════════════════════════ DAFTAR KONTAK ══════════════════════════╣")` <br>
`        P(" ╠══════════════════╦══════════════════╦═══════╦═══════╦═══════╦═══════╣")` <br>
`        P(" ║      NAMA        ║       NIM        ║ TUGAS ║  UTS  ║  UAS  ║ AKHIR ║")` <br>
`        P(" ╠══════════════════╬══════════════════╬═══════╬═══════╬═══════╬═══════╣")` <br>
`        for l in i:` <br>
`            if l == '':` <br>
`                pass` <br>
`            else:` <br>
`                l1 = l.replace('Nama : ','').replace('Nim : ','').replace('Tugas : ','').replace('UTS : ','').replace('UAS : ','').replace('Akhir : ','')` <br>
`                na,ni,tu,uts,uas,akhir = l1.strip().split('|')` <br>
`                P((' ║ ')+(na[:15]).ljust(17,'.')+('║ ')+(ni).ljust(17)+('║ ')+(tu).ljust(6)+('║ ')+(uts).ljust(6)+('║ ')+(uas).ljust(6)+('║ ')+(akhir).ljust(6)+('║'))` <br>
`        P(" ╚══════════════════╩══════════════════╩═══════╩═══════╩═══════╩═══════╝")` <br>
`    elif c.lower() == 'c':` <br>
`        cari = input(' Mencari : ')` <br>
`        i = open('database.txt','r').read().splitlines()` <br>
`        P(" ╔═════════════════════════════════════════════════════════════════════╗")` <br>
`        P(" ╠════════════════════════════ DAFTAR KONTAK ══════════════════════════╣")` <br>
`        P(" ╠══════════════════╦══════════════════╦═══════╦═══════╦═══════╦═══════╣")` <br>
`        P(" ║      NAMA        ║       NIM        ║ TUGAS ║  UTS  ║  UAS  ║ AKHIR ║")` <br>
`        P(" ╠══════════════════╬══════════════════╬═══════╬═══════╬═══════╬═══════╣")` <br>
`        for l in i:` <br>
`            if l == '':` <br>
`                pass` <br>
`            elif cari in l:` <br>
`                l1 = l.replace('Nama : ','').replace('Nim : ','').replace('Tugas : ','').replace('UTS : ','').replace('UAS : ','').replace('Akhir : ','')` <br>
`                na,ni,tu,uts,uas,akhir = l1.strip().split('|')` <br>
`                P((' ║ ')+(na).ljust(17)+('║ ')+(ni).ljust(17)+('║ ')+(tu).ljust(6)+('║ ')+(uts).ljust(6)+('║ ')+(uas).ljust(6)+('║ ')+(akhir).ljust(6)+('║'))` <br>
`        P(" ╚══════════════════╩══════════════════╩═══════╩═══════╩═══════╩═══════╝")` <br>
`    elif c.lower() == 'h':` <br>
`        u = open('database.txt','r').read().splitlines()` <br>
`        target = input(' Masukan Nama : ')` <br>
`        nm = []` <br>
`        for l in u:` <br>
`            if l == '':` <br>
`                pass` <br>
`            else:` <br>
`                l1 = l.replace('Nama : ','').replace('Nim : ','').replace('Tugas : ','').replace('UTS : ','').replace('UAS : ','').replace('Akhir : ','')` <br>
`                na,ni,tu,uts,uas,akhir = l1.strip().split('|')` <br>
`                if str(na) == str(target):` <br>
`                    P('BERHASIL MENGHAPUS Data %s'%(target))` <br>
`                    pass` <br>
`                else:` <br>
`                    nm.append(str(l)+'\n')` <br>
`        new = open('database.txt','w')` <br>
`        new.write(str(nm))` <br>
`        new.close()` <br>
`        new = open('database.txt','r').read().splitlines()` <br>
`        new1 = open('database.txt','w')` <br>
`        new1.close()` <br>
`        new2 = open('database.txt','a')` <br>
`        for i in new:` <br>
`            i2 = i.replace("['","").replace("\\n', '", "\n").replace("']","").replace("\\n",'')` <br>
`            new2.write(i2)` <br>
`        new2.close()` <br>
`    elif c.lower() == 'u':` <br>
`        u = open('database.txt','r').read().splitlines()` <br>
`        target = input(' Masukan Nama : ')` <br>
`        nm = []` <br>
`        for l in u:` <br>
`            if l == '':` <br>
`                pass` <br>
`            else:` <br>
`                l1 = l.replace('Nama : ','').replace('Nim : ','').replace('Tugas : ','').replace('UTS : ','').replace('UAS : ','').replace('Akhir : ','')` <br>
`                na,ni,tu,uts,uas,akhir = l1.strip().split('|')` <br>
`                if na == target:` <br>
`                    P(' Mengedit Data %s'%(target))` <br>
`                    while (True):` <br>
`                        nama = input(" Nama : ")` <br>
`                        if nama == '':` <br>
`                            P(' Masukan dengan Nama Dengan Benar')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            nim  = int(input(" NIM  : "))` <br>
`                            if nim == '':` <br>
`                                P(' Masukan Nim dengan Angka')` <br>
`                        except ValueError:` <br>
`                            P(' Masukan Nim dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            tugas  = int(input(" TUGAS  : "))` <br>
`                            if tugas == '':` <br>
`                                P(' Masukan TUGAS dengan Angka')` <br>
`                        except ValueError:` <br>
`                            P(' Masukan TUGAS dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            uts  = int(input(" UTS  : "))` <br>
`                            if uts == '':` ,br
`                                P(' Masukan UTS dengan Angka')` <br>
`                        except ValueError:` <br>
`                            P(' Masukan UTS dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
`                    while (True):` <br>
`                        try:` <br>
`                            uas  = int(input(" UAS  : "))` <br>
`                            if uas == '':` <br>
`                                P(' Masukan UAS dengan Angka')` <br>
`                        except ValueError:` <br>
`                            P(' Masukan UAS dengan Angka')` <br>
`                        else:` <br>
`                            break` <br>
`                    akhir = round((float(tugas) * 0.3)+(float(uts) * 0.35)+(float(uas) * 0.35),2)` <br>
`                    edit  =('Nama : '+nama+'|Nim : '+str(nim)+'|Tugas : '+str(tugas)+'|UTS : '+str(uts)+'|UAS : '+str(uas)+"|Akhir : "+str(akhir)+'\n')` <br>
`                    nm.append(edit+'\n')` <br>
`                else:` <br>
`                    nm.append(str(l)+'\n')` <br>
`        new = open('database.txt','w')` <br>
`        new.write(str(nm))` <br>
`        new.close()` <br>
`        new = open('database.txt','r').read().splitlines()` <br>
`        new1 = open('database.txt','w')` <br>
`        new1.close()` <br>
`        new2 = open('database.txt','a')` <br>
`        for i in new:` <br>
`            i2 = i.replace("['","").replace("\\n', '", "\n").replace("']","").replace("\\n","\n")` <br>
`            new2.write(i2+'\n')` <br>
`        new2.close()` <br>
`    elif c.lower() == 't':` <br>
`        i = open('database.txt','a')` <br>
`        P(" Tambah Kontak")` <br>
`        while (True):` <br>
`            nama = input(" Nama : ")` <br>
`            if nama == '':` <br>
`                P(' Masukan dengan Nama Dengan Benar')` <br>
`            else:` <br>
`                break` <br>
`        while (True):` <br>
`            try:` <br>
`                nim  = int(input(" NIM  : "))` <br>
`                if nim == '':` <br>
`                    P(' Masukan Nim dengan Angka')` <br>
`            except ValueError:` <br>
`                P(' Masukan Nim dengan Angka')` <br>
`            else:` <br>
`                break` <br>
`        while (True):` <br>
`            try:` <br>
`                tugas  = int(input(" TUGAS  : "))` <br>
`                if tugas == '':` <br>
`                    P(' Masukan TUGAS dengan Angka')` <br>
`            except ValueError:` <br>
`                P(' Masukan TUGAS dengan Angka')` <br>
`            else:` <br>
`                break` <br>
`        while (True):` <br>
`            try:` <br>
`                uts  = int(input(" UTS  : "))` <br>
`                if uts == '':` <br>
`                    P(' Masukan UTS dengan Angka')` <br>
`            except ValueError:` <br>
`                P(' Masukan UTS dengan Angka')` <br>
`            else:` <br>
`                break` <br>
`        while (True):` <br>
`            try:` <br>
`                uas  = int(input(" UAS  : "))` <br>
`                if uas == '':` <br>
`                    P(' Masukan UAS dengan Angka')` <br>
`            except ValueError:` <br>
`                P(' Masukan UAS dengan Angka')` <br>
`            else:` <br>
`                break` <br>
`        akhir = round((float(tugas) * 0.3)+(float(uts) * 0.35)+(float(uas) * 0.35),2)` <br>
`        i.write('\nNama : '+nama+'|Nim : '+str(nim)+'|Tugas : '+str(tugas)+'|UTS : '+str(uts)+'|UAS : '+str(uas)+"|Akhir : "+str(akhir)+'\n')` <br>
`        i.close()` <br>
`    else:` <br>
`        P("Silahkan pilih menu yang tersedia...")`

# Hasil dari source code di atas : <br>
!