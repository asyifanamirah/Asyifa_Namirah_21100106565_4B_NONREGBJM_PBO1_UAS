# Proyek Akhir Pemrograman Berbasis Objek 1

Proyek ini adalah contoh sederhana aplikasi pengolahan data tokokain menggunakan Java sebagai tugas akhir dari mata kuliah pemrograman berbasis objek 1.

## Deskripsi

Aplikasi ini menerima input berupa jenis danharga kain, dan memberikan output berupa informasi detail dari Kain tersebut seperti jenis, warna, harga, dan motif kain.

Aplikasi ini mengimplementasikan beberapa konsep penting dalam pemrograman berorientasi objek (OOP) seperti Class, Object, Atribut, Method Constructor, Method Mutator, Method Accessor, Encapsulation, Inheritance, Overloading, Overriding, Seleksi, Perulangan, IO Sederhana, Array, dan Error Handling.

## Penjelasan Kode

Berikut adalah bagian kode yang relevan dengan konsep OOP yang dijelaskan:

1. **Class** adalah template atau blueprint dari object. Pada kode ini, `Tokokain`, `Detailkain`, dan `TokoKainBersama` adalah contoh dari class.

```bash
public class Tokokain {
    ...
}

public class Detailkain extends Tokokain {
    ...
}

public class TokoKainBersama {
    ...
}
```

2. **Object** adalah instance dari class. Pada kode ini, `kain[i] = new Detailkain(jenis, harga);` adalah contoh pembuatan object.

```bash
kain[i] = new Detailkain(jenis, harga);
```

3. **Atribut** adalah variabel yang ada dalam class. Pada kode ini, `jenis` dan `harga` adalah contoh atribut.

```bash
String jenis;
String harga;
```

4. **Constructor** adalah method yang pertama kali dijalankan pada saat pembuatan object. Pada kode ini, constructor ada di dalam class `TokoKain` dan `Detailkain`.

```bash
public Tokokain(String jenis, String harga) {
    this.jenis = jenis;
    this.harga = harga;
}

public Detailkain(String jenis, String harga) {
    super(jenis, harga);
}
```

5. **Mutator** atau setter digunakan untuk mengubah nilai dari suatu atribut. Pada kode ini, `setjenis` dan `setharga` adalah contoh method mutator.

```bash
public void setjenis(String jenis) {
    this.jenis = jenis;
}

public void setharga(String harga) {
    this.harga = harga;
}
```

6. **Accessor** atau getter digunakan untuk mengambil nilai dari suatu atribut. Pada kode ini, `getjenis`, `getharga`, `getnopesanan`, `getkodepesanan`, dan `getkodepesanan` adalah contoh method accessor.

```bash
public String getjenis() {
    return jenis;
}

public String getharga() {
    return harga;
}
```

7. **Encapsulation** adalah konsep menyembunyikan data dengan membuat atribut menjadi private dan hanya bisa diakses melalui method. Pada kode ini, atribut `jenis` dan `harga` dienkapsulasi dan hanya bisa diakses melalui method getter dan setter.

```bash
private String jenis;
private String harga;
```

8. **Inheritance** adalah konsep di mana sebuah class bisa mewarisi property dan method dari class lain. Pada kode ini, `Detailmahasiswa` mewarisi `Tokokain` dengan sintaks `extends`.

```bash
public class Detailkain extends tokokain {
    ...
}
```

9. **Polymorphism** adalah konsep di mana sebuah nama dapat digunakan untuk merujuk ke beberapa tipe atau bentuk objek berbeda. Ini memungkinkan metode-metode dengan nama yang sama untuk berperilaku berbeda tergantung pada tipe objek yang mereka manipulasi, polymorphism bisa berbentuk Overloading ataupun Overriding. Pada kode ini, method `displayInfo(String)` di `Mahasiswa` merupakan overloading method `displayInfo` dan `displayInfo` di `MahasiswaDetail` merupakan override dari method `displayInfo` di `Mahasiswa`.

```bash
public String displayInfo(String pesanan) {
    return displayInfo() + "\npesanan: " + pesanan;
}

@Override
public String Infopesanan() {
    ...
}
```

10. **Seleksi** adalah statement kontrol yang digunakan untuk membuat keputusan berdasarkan kondisi. Pada kode ini, digunakan seleksi `if else` dalam method `getjenis` dan seleksi `switch` dalam method `getharga`.

```bash
public String getkodepesanan() {
    if(getjenis().substring(2, 4).equals("10")){
        return "Kain sasirangan";
    } else {
        return "kain lain";
    }

    //return getjenis().substring(2, 4).equals("10") ? "Kain Sasirangan" : "kain lain";
}

public String getProdi() {
    switch(getjenis().substring(4, 6)) {
        case "01":
            return "Kain Sasirangan";
        case "02":
            return "Kain Denim";
        case "03":
            return "Kain Batik";
        default:
            return "kain lain";
    }
}
```

11. **Perulangan** adalah statement kontrol yang digunakan untuk menjalankan blok kode berulang kali. Pada kode ini, digunakan loop `for` untuk meminta input dan menampilkan data.

```bash
for (int i = 0; i < kain.length; i++) {
    ...
}
```

12. **Input Output Sederhana** digunakan untuk menerima input dari user dan menampilkan output ke user. Pada kode ini, digunakan class `Scanner` untuk menerima input dan method `System.out.println` untuk menampilkan output.

```bash
Scanner scanner = new Scanner(System.in);
System.out.print("Masukkan Pesanan ke-" + (i + 1) + ": ");
String jenis = scanner.nextLine();

System.out.println("\nData kain:");
System.out.println(kain.infopesanan());
```

13. **Array** adalah struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel. Pada kode ini, `Detailkain[]jenis = new Detailkain[2];` adalah contoh penggunaan array.

```bash
Detailkain[] kain = new Detailkain[2];
```

14. **Error Handling** digunakan untuk menangani error yang mungkin terjadi saat runtime. Pada kode ini, digunakan `try catch` untuk menangani error.

```bash
try {
    // code that might throw an exception
} catch (Exception e) {
    System.out.println("Error: " + e.getMessage());
}
```

## Usulan nilai

| No  | Materi         |  Nilai  |
| :-: | -------------- | :-----: |
|  1  | Class          |    5    |
|  2  | Object         |    5    |
|  3  | Atribut        |    5    |
|  4  | Constructor    |    5    |
|  5  | Mutator        |    5    |
|  6  | Accessor       |    5    |
|  7  | Encapsulation  |    5    |
|  8  | Inheritance    |    5    |
|  9  | Polymorphism   |   10    |
| 10  | Seleksi        |    5    |
| 11  | Perulangan     |    5    |
| 12  | IO Sederhana   |   10    |
| 13  | Array          |   15    |
| 14  | Error Handling |   15    |
|     | **TOTAL**      | **100** |

## Pembuat

Nama:  Asyifa Namirah
NPM: 2110010565
