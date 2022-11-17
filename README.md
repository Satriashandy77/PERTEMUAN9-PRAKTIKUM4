# Pertemuan9-praktikum4

Repository ini dibuat untuk memenuhi tugas Pertemuan 9-Bahasa Pemrograman (Module Praktikum 4)

NAMA  : Shandy Satria Mandala
KELAS : TI.22.B1
NIM   : 312210173
DOSEN : Agung Nugroho
MK    : Bahasa Pemrograman

Pada halaman ini (Tugas Pertemuan-9-Module Praktikum 4) Dosen memberi tugas sebagai berikut :
Ada dua bahan praktik dimodule 4 kali ini yaitu :

  * Soal Latihan yang ada pada module praktikum 4
  
    ![SoalLatihan 1](https://user-images.githubusercontent.com/115962377/202339932-d6966d8a-ba07-4e01-bc5f-84114585eb7a.png)
    
  * Berikut ini saya menuliskan syntax sekaligus menuliskan langkah-langkahnya sebagai berikut
  
    ```python
    # membuat list print
    ("Buat sebuah list sebanyak 5 elemen dengan nilai bebas")
    list = [1, 2, 3, 4, 5] print(list)
    
    # mengakses list
    print("Menampilkan elemen 3")
    print(list[2])
    
    print("ambil nilai elemen 2 sampai ke 4")
    print(list[1:4])
    
    print("ambil elemen terakhir")
    print(list[-1])
    
    # mengubah elemen list
    print("ubah elemen 4 dengan nilai lainnya")
    list[4]=10
    print(list[3])
    
    print("ubah elemen 4 sampai dengan elemen terakhir")
    list[4:5]=[20,11]
    print(list)
    
    # Tambah elemen list
    print("Ambil 2 bagian dari list pertama(A) dan jadikan list ke 2(B)")
    list_pertama=list[3:5]
    print(list_pertama)
    
    print("tambah list B dengan nilai string")
    list_pertama.append("guest")
    print(list_pertama)
    
    print("Tambah list B dengan 3 nilai")
    list_pertama.append(["guest",7,8])
    print(list_pertama)
    
    print("Menggabungkan list B dengan list A")
    gabung=list_pertama+list
    print(gabung)
    
  * Berikut hasil run syntax untuk memenuhi latihan module 4 diatas :
  
    ![Hasil1_1 1](https://user-images.githubusercontent.com/115962377/202346088-550da06d-181a-4bb7-b972-4ea65b3a7867.png)

  * Soal Tugas Praktikum module 4
  
    ![Tugas_Pratikum 1](https://user-images.githubusercontent.com/115962377/202346445-4ddc22b4-88df-4cb8-a910-8916d5ea950b.png)

  * Pada soal tugas ini saya akan menuliskan dan menjelaskan syntax yang saya buat sebagai berikut :
  
    ```python
    print("===================================================================")
    print("Nama        : Shandy Satria Mandala")
    print("NIM         : 312210173")
    print("Kelas       : TI.22.B1")
    print("Mata Kuliah : Bahasa Pemrograman")
    print("===================================================================")
    print("Tugas Praktikum module 4")
    
    # Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut: • Progam meminta
    # memasukkan data sebanyak-banyaknya (gunakan perulangan) • Tampilkan pertanyaan untuk menambah data (y/t?),
    # apabila jawaban t (Tidak), maka program akan menampilkan daftar datanya. • Nilai Akhir diambil dari perhitungan 3
    # komponen nilai (tugas: 30%, uts: 35%, uas: 35%) • Buat flowchart dan penjelasan programnya pada README.md. • Commit
    # dan push repository ke github.
    
    from prettytable import PrettyTable
    
    baris = []
    stop = False
    
    # masukan nilai
    while (not stop):
        nama = input("Masukan Nama : ")
        nim = input("Masukan NIM : ")
        tugas = input("Masukan Nilai Tugas : ")
        uts = input("Masukan Nilai UTS : ")
        uas = input("Masukan Nilai UAS : ")
        nilai_akhir = 0.3 * float(tugas) + 0.35 * float(uts) + 0.35 * float(uas)
        baris.append([nama, nim, tugas, uts, uas, nilai_akhir])

        tanya = input("Tambah data? (y/n) : ")
        if (tanya == "n"):
            stop = True
        
    # cetak nilai
    print("===================================================================")
        
    x = PrettyTable()
    no = 0
        
    for isi in baris:
        no += 1
        x.field_names = ["No", "Nama", "Nim", "Tugas", "UTS", "UAS", "Nilai Akhir"]
        x.add_row([no, isi[0], isi[1], isi[2], isi[3], isi[4], isi[5]])
    print(x)
    
  * Flowchart program diatas adalah sebagai berikut :
  
    ![Flowchart 1](https://user-images.githubusercontent.com/115962377/202350626-8d85d3be-da6e-45ea-8e3c-1342477c5130.png)

Penjelasan singkat tentang fungsi While untuk mengatur kondisi seperti while not stop dan jika tidak berhenti maka system akan terus menampilkan perintah user untuk meninputkan data . Untuk perhitungan nilai akhir sesuai ketentuan yang dosen inginkan. Sedangkan untuk menampilkan hasil dari inputan user tersebut menggunakan fungsi/module yang ada pada PrettyTable bisa mengakses link berikut ini untuk panduan installation :
How to install PIP
How to install PrettyTable
How to install Numpy

# Demikian tugas module 4 pada pertemuan 9 yang bisa saya sampaikan

# TERIMAKASIH :)
  
    
    
