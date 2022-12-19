# UAS-Dasprog-B

# Ujian Akhir Semester 
<br>Mata Kuliah 	: DASAR PEMOGRAMAN
<br> Nama		: Muhammad Azfa Haqqoni
<br>NIM		:	1227050086
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

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
  
  ![Screenshot_20221219_150956](https://user-images.githubusercontent.com/121001743/208379508-142dce10-adc5-4f3c-97dc-6e71859e9634.png


