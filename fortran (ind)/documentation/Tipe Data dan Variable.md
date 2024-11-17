

## catatan penting
semua deklarasi harus dilakukan sebelum operasi apapun
contoh akan error:
```

program example
  implicit none

  integer :: i
  real :: x

  print *, "Enter a number:"
  read *, x

  integer :: n  ! ini bakal error ===========
  n = int(x)
  do i = 1, n
    real :: y  ! ini juga ==========
    y = x * i
    print *, y
  end do

end program example
```
sehingga harusnya seperti ini
```
program example
  implicit none
  integer :: i
  real :: x
  integer :: n  !aman ==========
  real :: y  ! aman ============
  print *, "Enter a number:"
  read *, x
  
  n = int(x)
  do i = 1, n
    y = x * i
    print *, y
  end do

end program example
```
## Tipe data
Tipe data merupakan informasi tipe suatu data dimana hal ini akan memberi tahu baik komputer maupun manusia tipe apa yang sedang / dideklarasikan pada suatu variable, hal ini juga membantu komputer untuk mengetahui ukuran alamat yang digunakan untuk menyimpan data

deklarasi tipe data pada fortran ditulis dengan sintaks sebagai berikut:
\<tipe data\> :: <variable_name>

dengan tipe data built in pada fortran sebagai berikut:
-  `integer` – yaitu data representasi **bilangan bulat** negatif maupun positif 
    
- `real` – untuk bilangan float, atau memiliki koma (3.14 , 7.5 , dll)
    
- `complex` – tipe data pasangan bilangan real dan imaginary (lupakan, ini gk terlalu dipake, keknya)
    
- `character` – menyimpan **sebuah karakter**  seperti 'A','&',dll
    
- `logical` – yaitu boolean atau nilai benar atau salah (true or false)


lalu bagaimana dengan **string?** , kita tahu bahwa sebuah string/kalimat/kata adalah kumpulan dari karakter bukan? contoh:
"jokowi" terdiri dari = 'j' 'o' 'k' 'o' 'w' 'i'
nah maka dengan kata **kumpulan** , bisa kita simpulkan untuk membuat suatu string maka memerlukan sebuah array/list untuk menjadikan kumpulan karakter menjadi string

jadi string bisa direpresentasikan tipe data sebagai berikut:
- character(len=10)
- character(len=*)
- character(:)

lebih lanjut pada materi array dan string  [[array dan string]]
