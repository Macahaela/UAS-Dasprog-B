# Ujian Akhir Semester 
<br>Mata Kuliah 	:Dasar Pemrograman
<br> Nama		      :Michael
<br>NIM		        :1227050071
<br>Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, seperti contoh berikut:
int arr[2][2];
Untuk UAS kali ini kami diminta membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris sedangkan program ke dua digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.

## Source Code 1
    #include <iostream>
    using namespace std;

    int main(){
      cout<<"Nama  : Michael"<<endl;
      cout<<"NIM   : 1227050071"<<endl;
      cout<<"Kelas : IF-B"<<endl;
      cout<<endl;

      int i, j, m, n, matriks[10][10], transpose[10][10];

      cout << "Masukkan Jumlah Baris : ";
      cin >> n;
      cout << "Masukkan Jumlah Kolom : ";
      cin >> m;

      cout << "Masukkan Nilai: " << endl;
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

      cout << "Hasil Pertukaran Matriks: \n";
      for (i = 0; i < n; i++){
        for (j = 0; j < m; j++){
          cout << transpose[i][j] << "\t";
        }
        cout << endl;
      }
    }
    
## Source Code 2
    #include <iostream>
    using namespace std;

    const int MAX_ROWS = 100;
    const int MAX_COLS = 100;

    int main()
    {
      cout << "Nama  : Michael" << endl;
      cout << "NIM   : 1227050071 " << endl;
      cout << "Kelas : IF-B" << endl;
      cout << "==========================================" << endl;
      cout << "    Program C++ Input Matriks 2 Dimensi   "   << endl;
      cout << "==========================================" << endl;

      int array[MAX_ROWS][MAX_COLS];
      int rows, cols;

      cout << "Masukkan Jumlah Baris Array: ";
      cin >> rows;
      cout << "Masukkan Jumlah Kolom Array: ";
      cin >> cols;

      cout << "Masukkan Nilai Array: " << endl;
      for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
          cin >> array[i][j];
        }
      }

      cout << "Bilangan Yang Habis Dibagi 3, 5, dan 7: " << endl;
      for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
          if (array[i][j] % 3 == 0 && array[i][j] % 5 == 0 && array[i][j] % 7 == 0) {
            cout << array[i][j] << " ";
          }
        }
      }

      return 0;
    }
    
## Output 1
![Screenshot (20)](https://user-images.githubusercontent.com/120998463/208374000-f27fcec3-4e15-41bf-badb-a993940619b9.png)

## Output 2
![Screenshot (21)](https://user-images.githubusercontent.com/120998463/208377487-f96d18b1-b23f-4931-80e1-14574360051b.png)
