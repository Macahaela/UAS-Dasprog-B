# Ujian Akhir Semester 
<br>Mata Kuliah 	:Dasar Pemrograman
<br> Nama		      :Michael
<br>NIM		        :1227050071
<br>Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code

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
## Output
![Screenshot (19)](https://user-images.githubusercontent.com/120998463/208372129-2718cd4c-037f-4329-a040-6f706b0db189.png)
