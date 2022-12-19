# UAS-Dasprog-B

# Ujian Akhir Semester 
<br>Mata Kuliah 	: DASAR PEMOGRAMAN
<br> Nama		: Muhammad Azfa Haqqoni
<br>NIM		:	1227050086
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, seperti contoh berikut:
int arr[2][2];
Untuk UAS kali ini kami diminta membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris sedangkan program ke dua digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.

## Source Code 1

        #include <iostream>
        using namespace std;

        int main(){
          cout<<"Nama  : Muhammad Azfa Haqqoni"<<endl;
          cout<<"NIM   : 1227050086"<<endl;
          cout<<"Kelas : IF-B"<<endl;
          cout<<endl;

          int i, j, m, n, matriks[10][10], transpose[10][10];

          cout << "Masukkan jumlah baris yang diinginkan: ";
          cin >> m;
          cout << "Masukkan jumlah kolom yang diinginkan: ";
          cin >> n;

          cout << "Masukkan nilai\n";
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              cin  >> matriks[i][j];
            }
          }

          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              transpose[j][i] = matriks[i][j];
            }
          }

          cout << "Hasil pertukaran Matriks: \n";
          for (i = 0; i < n; i++){
            for (j = 0; j < m; j++){
              cout << transpose[i][j] << "\t";
            }
            cout << endl;
          }
        } 
   

## Output 1
![Screenshot_20221219_144349](https://user-images.githubusercontent.com/121001743/208378813-d08eff88-99d0-4375-90c5-e5171eb9ed9f.png)

## Source Code 2

#include <iostream>
using namespace std;

const int MAX_ROWS = 100;
const int MAX_COLS = 100;

int main()
{
  cout << "^Nama  : Muhammad Azfa Haqqoni" << endl;
  cout << "^NIM   : 1227050086 " << endl;
  cout << "^Kelas : IF-B" << endl;
  cout << "==========================================" << endl;
  cout << "^Program C++ Input Matriks 2 Dimensi^" << endl;
  cout << "==========================================" << endl;
  cout << endl;
  
  int array[MAX_ROWS][MAX_COLS];
  int rows, cols;

  cout << "Masukkan jumlah baris array: ";
  cin >> rows;
  cout << "Masukkan jumlah kolom array: ";
  cin >> cols;

  cout << "Masukkan elemen-elemen array: " << endl;
  for (int i = 0; i < rows; i++) {
    for (int j = 0; j < cols; j++) {
      cin >> array[i][j];
    }
  }

  cout << "Bilangan yang habis dibagi 3, 5, dan 7: " << endl;
  for (int i = 0; i < rows; i++) {
    for (int j = 0; j < cols; j++) {
      if (array[i][j] % 3 == 0 && array[i][j] % 5 == 0 && array[i][j] % 7 == 0) {
        cout << array[i][j] << " ";
      }
    }
  }

  return 0;
}
  

## Output 2

![Screenshot_20221219_150956](https://user-images.githubusercontent.com/121001743/208424208-2ec095e1-510e-4918-b9bb-b55bdb11d126.png)



