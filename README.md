# ORIENTED OBJECT PROGRAMMING
## Pra_Praktikum3


### Membuat Superclass Manusia dengan atribut Private
      public class Manusia {
          private String nama;
          private String jenisKelamin;
          private int umur;
          private String alamat;


          //Menggunakan Setter untuk atribut private
          public void setNama(String nama) {
              this.nama = nama;
          }
          public void setJenisKelamin(String jenisKelamin) {
              this.jenisKelamin = jenisKelamin;
          }
          public void setUmur(int umur) {
              this.umur = umur;
          }
          public void setAlamat(String alamat) {
              this.alamat = alamat;
          }

          //Menggunakan Getter untuk atribut private
          public String getNama() {
              return nama;
          }
          public String getJenisKelamin() {
              return jenisKelamin;
          }
          public int getUmur() {
              return umur;
          }
          public String getAlamat() {
              return alamat;
          }
          
          public void cetakInfoManusia() {
              System.out.println("Nama : " + getNama());
              System.out.println("Jenis Kelamin : " + getJenisKelamin());
              System.out.println("Umur : " + getUmur());
              System.out.println("Alamat : " + getAlamat());
          }
      }
      
###
### Membuat Subclass Mahasiswa
      public class Mahasiswa extends Manusia {
          private int nim;
          private String jurusan;

          // Menggunakan Setter Karena atribut Private
          public void setNim(int nim) {
              this.nim = nim;
          }

          public void setJurusan(String jurusan) {
              this.jurusan = jurusan;
          }

          // Menggunakan Getter Karena atribut Private
          public int getNim() {
              return nim;
          }

          public String getJurusan() {
              return jurusan;
          }

          //Membuat method untuk menampilkan data mahasiswa
          public void cetakInfoMahasiswa() {
              System.out.println("Nama          : " + getNama());
              System.out.println("NIM           : " + getNim());
              System.out.println("Jurusan       : " + getJurusan());
              System.out.println("Jenis Kelamin : " + getJenisKelamin());
              System.out.println("Umur          : " + getUmur());
              System.out.println("Alamat        : " + getAlamat());

          }

          public static void main(String[] args){

                  // Membuat object
                  Mahasiswa anton = new Mahasiswa();

                  /* memanggil atribut dan memberi nilai */
                  anton.setNim(10102020);
                  anton.setNama("Anton Santoso");
                  anton.setJenisKelamin("Laki-laki");
                  anton.setUmur(28);
                  anton.setAlamat("Bekasi Kota");
                  anton.setJurusan("Informatika");

                  anton.cetakInfoMahasiswa();
              }

      }
![Screenshot (12)](https://user-images.githubusercontent.com/115928747/199939702-2f792227-51d7-4c28-8185-ba7274050657.png)
