FORTRAN (sebelumnya dikenal sebagai **FORmula TRANslation**) adalah bahasa pemrograman tingkat tinggi yang dirancang terutama untuk komputasi ilmiah dan teknik. Ciri utamanya adalah kemampuannya untuk menangani operasi numerik dengan efisiensi tinggi.

## indentation type
Fortran adalah bahasa yang memiliki gaya indentation sebagai tanda bahwa block of code itu, beberapa jenis code juga memiliki statement "end \<code\>"
dimana bertujuan memberi info bahwa itu adalah akhir dari code dan indentation membernya,.
contoh:

```
code 1:
	#start
	block of code 
	...
	#end, maka dari start-end adalah bagian dari code 1
	#sehingga eksekusi block of code tergantung pada kondisi code 1
end code 1
```


## Data type explicity
Tipe data di fortran dideklarasikan secara implicit maupun eksplisit dimana kita bisa menentukan apakah tipe data tiap variabel ditentukan di awal atau tidak.
contoh:
```
#implicit none
integer::variable=6

#implicit activated
variable=6

```
bisa kita lihat bahwa pada *implicit none* variable ditambahkan kata *integer* untuk menunjukkan bahwa variable tersebut bertipe data integer, dan seterusnya

sedangkan pada *implicit activated*  variable tidak perlu ditambahkan tipe data dibelakangnya, namun hal ini akan lebih berbahaya untuk tingkat eror dan keamanan kode kedepannya





