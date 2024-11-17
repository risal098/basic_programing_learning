array adalah sebuah tipe data atau tempat penyimpanan yang hanya menyimpan 1 jenis tipe data dan memiliki ukuran yang fix/tidak bisa diubah sampai akhir hayat


## Deklarasi array dan string


deklarasi array memiliki sintaks sebagai berikut:
```
<variable_type>::dimension(<ukuran_array>,...banyak_dimensi)::array
```

contoh:
- **integer,dimension(10)::array1** 
// maka artinya array1 menanpung 10 item dan hanya 1 dimensi \[item1,item2,item3]

- **integer,dimension(10,10)::matrix10_10** 
//artinya matrix10_10 menanpung 10 array yang masing masing berukuran max 10 item, jadi maksudnya bisa dibilang juga matrix 10 x 10

contoh deklarasi/aturan lain sebagai berikut:

- integer```
```
		- integer :: variable_name(<ukuran_array>,...banyak_dimensi)
		- integer :: variable_name(<panjang\>)=\[1,2,3...panjang]
```
- character / string
```
		- character(len=10) ::variable_name //panjang string hanya 10, jadi 
			lebih dri itu akan di potong, kurang dari itu akan auto padding
		- character(10)::variable_name // panjang string juga 10, sama kyk diatas
		- character(:),allocateable::variable_name // panjang akan mengikuti 
			inisiasi nanti
```


