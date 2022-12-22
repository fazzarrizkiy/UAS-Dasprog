# Ujian Akhir Semester 
<br>Mata Kuliah 	:Dasar Pemrograman
<br> Nama		: Muhamad Fazar Rizky Ardianto
<br>NIM		:	1227050077
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br> soal 1
<br> Pada soal pertama kita diharuskan mengubah/transpose sebuah matriks dengan mengubah kolom menjadi garis dan begitupun sebaliknya, dengan baris,kolom & nilai indexnya di inputkan.
## Source Code
```
#include <iostream>
using namespace std;

int main(){
  int i, j, bar, kol, matriks[10][10], transpose[10][10];

do{
  cout << "Masukkan jumlah baris matriks: ";
  cin >> bar;
  cout << "Masukkan jumlah kolom matriks: ";
  cin >> kol;
}
while (bar>10||kol>10);
  cout << "Masukkan elemen matriks\n";
  for (i = 0; i < bar; i++){
    for (j = 0; j < kol; j++){
      cout <<"matriks [" << i << "," << j << "] = ";
      cin  >> matriks[i][j];
    }
  }

cout<<endl;
cout << "Matriks" << endl;
for(i=0; i< bar; i++){
for(j=0; j<kol; j++){
cout <<matriks[i][j];
cout<< " ";
}
cout<<endl;
}

  for (i = 0; i < bar; i++){
    for (j = 0; j < kol; j++){
      transpose[j][i] = matriks[i][j];
    }
  }

  cout << "Hasil Transpose Matriks:"<<endl;
  for (i = 0; i < kol; i++){
    for (j = 0; j < bar; j++){
    cout << transpose[i][j] << "\t";
    }
    cout << endl;
  }
}
```
## Output
```
![image](https://user-images.githubusercontent.com/119167491/209126860-253b7a5e-3280-404d-b8b0-b61b9668de34.png)

```
<br>pada pemrograman ini dilakukan perubahan atau transpose matriks dimana index yang dimasukan akan di kalkulasikan dan disusun seuai dengan transposenya. dimana pengulangan for berperan sebagai pemberi nilai index dan proses transpose.


## Deskripsi Umum
<br>pada soal 2 kita diharuskan mencari program dimana setiapa angka yang di inputkan dapat dibagi habis dengan 3, 5 & 7 dan akan tersusun pada matriks.
## Source Code
```
#include <iostream>
using namespace std;

int main(){
  int i,j; 
  int baris, kolom; 
  int matriks[100][100];
  
  cout<<"mencari nilai yang habis dibagi 3,5 & 7"<<endl;
  cout<<"====================================="<<endl;
  cout << "Masukkan baris matriks: ";
  cin >> baris;
  cout << "Masukkan kolom matriks: ";
  cin >> kolom;

  cout << "Masukkan elemen matriks"<<endl;
  for (i = 1; i <= baris; i++){
    for (j = 1; j <= kolom; j++){
      cout <<"matriks [" << i << "," << j << "] = ";
      cin  >> matriks[i][j];
    }
  }
  
  cout << "Matriks yang bilangannya habis 3,5,7 adalah : "<<endl;
  for (i = 1; i <= baris; i++){
  	for (j = 1; j <= kolom; j++){
  		if (matriks [i][j] % 3 == 0 or matriks [i][j] % 5 == 0 or matriks [i][j] % 7 == 0){
  			matriks [i][j] = matriks [i][j];
		  }
		else {
			matriks [i][j] = 0;
			
		}
	  }
  }
  for (i = 1; i <= baris; i++){
    for (j = 1; j <= kolom; j++){
      cout << matriks [i][j] << "\t";
    }
    cout << endl;
  }  
}
```
## Output 
```
![image](https://user-images.githubusercontent.com/119167491/209139327-759db8be-9bbc-4831-a054-ae2571aaf4c5.png)
```
<br>Output yang dihasilkan ialah ketika angka yang di inputkan dan bisa dibagi habis dengan 3,5&7 akan disusun pada matriks dimana angka yang bisa dibagi habis akan ditampilkan nilai angakanya sedangkan yang tidak bisa dibagi habis akan memiliki nilai 0.
