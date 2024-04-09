==================
Asas Python
==================
##  **Pengenalan Jupyter Notebook**

Mari berkenalan dengan Jupyter Notebook sebelum kita mula menulis kod.

Pada tajuk sebelum ini, penulisa ada menyarankan anda menggunakan Jupyter Notebook untuk permulaan. Sekarang, mari kita mempelajari serba sedikit tentang komponen dalam IDE ini.

Ikut langkah dibawah:

1. Klik pada ikon Anaconda di skrin komputer anda.
2. Tetingkap Anaconda akan terpapar dan dan klik pada Jupyter Notebook.
3. Jupyter akan dibuka dengan menggunakan tab daripada Chrome.
4. Klik pada **New** dan seterusnya pada **python3.**

-- gambar

5. Anda akan menemukan paparan yang menyediakan pentas untuk menulis kod Python.
-- gambar
Seterusnya mari berkenalan dengan paparan Jupyter Notebook.

1. Pada barisan ketiga, anda akan melihat terdapat beberapa ikon seperti disket, tambah, gunting dan sebagainya. Setiap ikon kecil ini mempunyai fungsi yang tersendiri.

-- gambar

| **Nombor** | **Fungsi** |
| ---- | ---- |
| **1** | Simpan |
| **2** | Tambah blok kod |
| **3** | Buang blok kod |
| **4** | Tiru blok kod |
| **5** | Tampal blok kod |
| **6** | Gerakkan blok keatas |
| **7** | Gerakkan blok kebawah |
| **8** | Jalankan kod |
| **9** | Hentikan kernel |
| **10** | Mula semula kernel |
| **11** | Mula semula kernal, jalankan semula kernel |
| **12** | Pilihan jenis blok |
| **13** | Buka palet arahan |

Terdapat banyak lagi fungsi lain dalam Jupyter Notebook, tetapi setakat ini, ini yang akan digunakan untuk pembelajaran seterusnya.

##  **Arahan**

Kita mulakan asas Python dengan memahami konsep _Commander and Command. Commander_ atau komander adalah satu pangkat gelaran yang biasanya diberikan kepada ketua dalam kumpulan askar. Komander akan memberikan arahan (_command_)  kepada askar dibawahnya untuk dilaksanakan.
 
Dalam konteks pengaturcaraan, anda adalah Komander tersebut.

Anda memberi arahan berbentuk barisan kod ke dalam IDE. Kemudian IDE akan membaca kod tersebut dan menjalankannya untuk menghasilkan output.

Untuk memahami dengan mendalam lagi konsep ini dengan cara yang lebih menyeronokkan, penulis mempelawa anda untuk bermain di pantai bersama si penyu! Dalam kod ini, anda akan mempelajari bagaimana ingin menggerakkan penyu. Disebabkan penyu berada di pantai,  pergerakkannya akan menyebabkan kesan pada permukaan dan itu membolehkan anda untuk melukis sesuatu.

Mari kita mulakan permainan ini.

1. Buka **Anaconda Command Prompt** (bukan CMD biasa) dan masukkan kod berikut baris demi baris. Mulakan dengan baris pertama dan klik (_enter_) kemudian kod seterusnya hingga baris akhir.

```
conda env list**
conda create -n turtle python=3.6**
conda activate turtle**
pip install mobilechelonian**
juypter notebook
```
2. Buka Jupyter Notebook dan cipta satu fail baru. Masukkan kod di bawah. Untuk permulaan, anda tidak perlu memahami kod ini secara mendalam. Cukup memahami kod ini adalah untuk mencipta penyu yang akan mengikut arahan anda.

```python
from mobilechelonian import Turtle
t = Turtle()
```
3. Klik Run dan visual dibawah akan terpapar seekor penyu yang mempunyai keupayaan untuk bergerak.

4. Anda tambah blok kod yang baharu dan cuba masukkan kod berikut.

```python
t.forward(100)
t.right(90)
```

Output:

-- gambar

Penyu akan bergerak kehadapan sejauh 100 pixel dan telah berputar 90 darjah ke kiri dari posisi asal. Anda sebagai komander telah memberi arahan bergerak ke hadapan dengan arahan **t.forward**(jarak bergerak) dan juga arahan membelok dengan arahan **t.left**(sudut membelok).

Penyu akan meninggalkan kesan warna hitam seperti dakwat lukisan apabila dia bergerak.

5. Selain daripada arahan kedepan dan membelok di atas, anda juga boleh mengarahkan penyu dengan arahan berikut;

| **Arahan** | **Maksud** |
| ---- | ---- |
| **t.backward(**_jarak_**)** | Arahan mengundur |
| **t.right (**_sudut_**)** | Arahan berputar ke kanan |
| **t.setposition(**_koordinat-x, koordinat-y_**)** | Arahan menetapkan posisi dalam nilai koordinat. (anda boleh menetapkan mod _grid_ pada tempat dimana penyu bermain untuk menentukan posisinya.) |
| **t.home( )** | Arahan untuk kembali semula ke titik mula. |
| **t.penup( )** | Arahan untuk berhenti melukis. (_pen up_ adalah seperti mengangkat pen dari kertas) |
| **t.pendown()** | Arahan untuk mula melukis. (_pen down_ adalah seperti meletakkan semula pen ke atas kertas.) |

6. Dengan sedikit kekreatifan, hanya dengan menggunakan arahan di atas, anda boleh melukis pelbagai bentuk seperti contoh dibawah!

-- gambar

Ini sedikit kerja penulis berikan buat anda. Cubalah!

Daripada subtopik ini, anda telah memahami bagaimana pengaturcaraan berfungsi dimana terdapat anda sebagai komander yang memberi arahan (_command_) di dalam kod anda. Kod tersebut akan melaksanakan apa yang anda kehendaki dengan syarat kod tersebut haruslah ditulis tanpa kesalahan padanya.

Setelah memahami tentang mekanisma mudah ini, ayuh kita lanjut kepada kod yang bertindak untuk menghasilkan _output_ akhir sesebuah kod iaitu, `print ()`.

##  **_Print Function_**

· **print ( )**

Kita mulakan asas Pythod dengan sesuatu yang mudah iaitu fungsi **print()****. 

Fungsi **print()** digunakan bagi merumuskan kod yang telah ditulis supaya _output_ daripada kod tersebut dapat dihasilkan. _Output_ adalah hasil akhir yang terhasil daripada kod yang telah ditulis.

Mari tulis kod pertama anda.

```python
>>> print("Hello dunia!")
Hello dunia!
```

Seperti _printer_, fungsi **print()** mengeluarkan output pada nilai yang diletakkan dalam kurungan fungsi ini.

Anda boleh meletakkan perkataan dan nombor untuk menghasilkan output. Cuba ubah perkataan di atas kepada nombor dan _run_ kod tersebut.

##  **Variable**

**Variable** adalah **nama** yang mewakili kepada **sesuatu nilai** dalam sesebuah kod. _Variable_ bersifat _case sensitive_ iaitu penggunaan aksara besar atau kecil memberi perbezaan kepada _variable_ tersebut.

Misalnya, **fruit** dan **Fruit** adalah sesuatu yang berbeza walaupun maknanya sama. Jadi anda haruslah berhati-hati ketika menulis kerana aksara besar dan kecil memberi makna berbeza kepada Python.

Di bawah adalah contoh _variable_.

```python
>>> kereta = 'wira'
>>> kereta_1 = 'saga'
>>> kereta_2 = 'bezza'
>>> proton = kereta + kereta_1 + kereta_2
>>> print (proton)**
wirasagabezza

```
Jika dilihat dalam kod diatas, maklumat nama kereta “wira”, “saga”, dan “bezza” telah disimpan ke dalam _variable_ bernama **kereta**, **kereta_1** dan **kereta_2**. Maklumat nama kereta ini telah diapit menggunakan pembuka dan penutup kata (“ “) dan ini mencipta sebuah **string**_._

Di barisan keempat, semua maklumat yang telah disimpan di dalam _variable_ disimpan ke dalam _variable_ **proton**.

_Variable_ juga boleh wujud dalam bentuk persamaan matematik. Contohnya persamaan garis lurus dan formula kecerunan,

**m = (y2 – y1) /(x2 – x1)**

**y = m*x + c**

**m** diatas merujuk kepada formula kecerunan dalam sistem koordinat. Maklumat **m** kemudian disimpan ke dalam maklumat **y** dimana **y** adalah sebuah persamaan garis lurus.

##  **String**

Di dalam tajuk sebelum ini iaitu _variable_, penulis ada menyebut beberapa kali perkataan _string_ dan telah mempunyai definisi iaitu apabila sesuatu perkataan diapit menggunakan pembuka dan penutup kata (“ “). Di dalam Python, s_tring_ boleh dimanipulasi dengan beberapa arahan yang telah ditetapkan. Ia dinamakan sebagai **metod string**.

Contoh,

1. Modifikasi –  memanipulasi _string_ kepada aksara besar dan kecil.

o variable.upper( )

o variable.lower( )

Contoh kod:
```python
>>> x = 'Nama penulis adalah Ahmad.'
>>> print(x.upper())
>>> print(x.lower())

NAMA penulis ADALAH AHMAD
nama penulis adalah ahmad
```
2. Penggabungan

Penggabungan _string_ mudah boleh dilakukan dengan dengan hanya menggunakan simbol tambah, **+**.

Contoh kod:
```python
>>> anak_1 = 'Ali'
>>> anak_2 = 'Abu'
>>> anak_mama = anak_1 + '&' + anak_2
>>> print(anak_mama)
Ali & Abu
```
3. Memformat string

· **string_{}.format(argument)**

Memformat string adalah sebuah metod mencipta sebuah templat kosong yang boleh diisi dengan apa-apa maklumat. Bagi menulis stail format, kurungan keriting (_curly bracket_) digunakan sebagai templat tempat kosong. Terdapat 2 cara untuk menulis metod ini.

Cara 1:
```python
>>> bahan_1 = 'ayam'
>>> print('Bahan ayam masak merah adalah {}'.format(bahan_1))
Bahan ayam masak merah adalah ayam
```
Cara 2:
```python
>>> bahan_1 = 'ayam'
>>> print(f'Bahan ayam masak merah adalah** **{bahan_1}')
Bahan ayam masak merah adalah ayam
```
##  **Interger**

Istilah **integer** daripada segi matematik adalah nombor yang tidak mempunyai nilai pecahan. Dalam bahasa mudahnya adalah nombor bulat. Contoh; 1, 23, 456, 3400. Nombor seperti 1.2, 31/2, 2(1/4) tidak termasuk dalam interger tetapi dalam **float**.

Integer boleh beroperasi dengan menggunakan operator matematik seperti proses tambah, tolak, bahagi, darab, kuasa, punca-kuasa, modulus dan lain lain.

Contoh kod:
```python
>>> a = 2
>>> b = 5
>>> print (a+b) # penambahan
>>> print((b-a) # tolak
>>> print(b*a) # darab
>>> print(b/a) # bahagi
>>>** **print(5 // 2) # (floor division)
>>> print(b % a) # modulus
7
3
10
2.5
2
1
```

Bagi **float** pula, terdapat perbezaan _output_ yang dihasilkan.

Contoh kod:
```python
>>> x = 0.
>>> y = 0.002
>>> print(x+y)
0.10200000000000001
```
Jika diperhatikan daripada _output_ kod di atas, jawapan yang terhasil adalah tidak seperti yang diharapkan iaitu, 0.102.  _Output_ yang diberikan pula panjang dan mempunyai banyak nilai sifar, diakhir dengan nilai 1.

Python membaca kod ini sebagai **float** atau kita namakan ia sebagai nombor awangan. Walaubagaimanapun, masalah ini boleh diselesaikan dengan fungsi **round()**. Format bagi fungsi **round()** adalah **round(**_jawapan akhir, nilai bundar_**)**.  Kod diatas boleh diperbaiki kepada berikut;

```python
>>> x = 0.1
>>> y = 0.002
>>> a = round(x + y, 3)
>>> print(a)
0.102
```
##  **Tuple, List, Dictionary, Set**

Pada tajuk yang lepas, kita telah mempelajari berkenaan **_variable_** iaitu satu nama yang digunakan untuk menyimpan maklumat seperti perkataan atau nombor.

Maklumat atau _data_ adalah sebuah asas yang sangat penting untuk difahami pada peringkat awal pembelajaran pengaturcaraan. Dalam Python, terdapat beberapa sturktur data yang digunakan yang mempunyai ciri tertentu yang sangat sesuai digunakan dalam banyak keadaan.

Data struktur itu ialah **tuple****,** **list****,** **dictionary** dan **set**. Setiap struktur data ini mempunyai ciri-ciri yang berbeza yang akan dinyatakan dengan lebih dalam pada tajuk seterusnya.

###  **Tuple** 

**Tuple** adalah sebuah kumpulan maklumat yang menggunakan **kurungan ( )** sebagai pembuka dan penutup senarai tersebut.

Contoh:
```python
>>> makanan = ('burger', 'sos', 'pizza', 'nasi)
>>> print(makanan)
('burger', 'sos', 'pizza', 'nasi)
```
String **'burger', 'sos', 'pizza'** dan **'nasi'** berada di dalam sebuah **Tuple**. **Tuple** tidak boleh diubahsuai, dikemaskini, dipadam kandungannya dengan arahan spesifik. (hanya boleh diubah daripada kod secara terus dengan memadam dan menulis semula). **Tuple** membenarkan maklumat yang sama berada dalam satu **tuple**.

###  **List** 

Struktur data seterusnya adalah **List** iaitu sebuah kumpulan maklumat yang menggunakan **kurungan petak [ ]** sebagai pembuka dan penutup kata. 

**List** juga berfungsi sebagai **array**; atau boleh difahami sebagai sebuah bekas atau fail untuk menyimpan maklumat. _List_ mempunyai ciri istimewa iaitu maklumat di dalam **List** akan dilabel dengan nombor INDEX (bermula dengan nilai sifar) yang menjadikan penyimpanan maklumat tadi lebih tersusun rapi.

Contoh:
```python
>>> minuman = ['sirap', 'laici', 'kopi', 'teh']
```

| **INDEX** | **string** |
| --------- | ---------- |
| [0]       | 'sirap',   |
| [1]       | 'laici'    |
| [2]       | 'kopi'     |
| [3]       | 'teh'      |

Berikut adalah cara untuk mengakses item dalam _list:_
```python
>>> print(minuman[0])
sirap
>>> print(minuman[1])
laici
```
_List_ boleh dimanipulasi dengan fungsi tertentu. Antaranya, memasukkan maklumat pada _index_ tertentu dengan menggunakan **insert()**, menambah maklumat dengan menggunakan **.append()**, membuang maklumat dengan menggunakan **remove()** ataupun **pop()**, menyusun secara terbalik maklumat dengan **reverse()**, dan lain lain lagi.

Contoh kod;
```python 
>>> minuman.insert(1, 'milo')
>>> print(minuman)
['sirap', 'milo', 'laici', 'kopi', 'teh']
```
```python
>>> minuman.append('limau_ais')
>>> print(minuman)
['sirap','laici', 'kopi', 'teh',]
```
```python
>>> minuman.remove('laici')
>>> print(minuman)
['sirap', 'kopi', 'teh']
```

###  **Set** 

**Set** adalah sebuah kumpulan maklumat yang menggunakan **kurungan keriting { }** sebagai kurungan.

**Set** tidak menggunakan **index** seperti **list** serta tidak tersusun kandungannya.

Contoh kod;
```python
>>> hari = {'isnin', 'selasa', 'rabu'}
>>> print (hari)
{'isnin', 'selasa', 'rabu'}
```

Ciri ciri _set_ adalah output yang akan terhasil dalam _set_ adalah unik dan tidak akan ada yang sama. Jadi jika anda ingin satu set data yang tidak mempunyai pendua, gunakan _set_ untuk mencipta output tersebut.

###  **Dictionary** 

_Dictionary_ juga menggunakan kurunga keriting seperti _set._ Perbezaannya dengan set (set hanya mempunyai value), **dictionary** menggunakan **key** sebagai rujukan kepada **value**.

Dibawah adalah contoh maklumat dalam bentuk _dictionary_.
```python
>>>test_dict = {"key":"value"}
>>>info = {"name":"Jack", "location":"USA"}
```
_Key_ yang sama tidak boleh digunakan secara berulang dalam _dictionary_. Untuk ciri-ciri pula, maklumat boleh ditambah, diubahsuai, dipadam dengan arahan sama seperti yang ada di dalam **list**.
```python
>>> hari = {"hari_1":"isnin","hari_2":'selasa' "hari_3":'rabu'}
>>> print(hari[‘hari_1’])
isnin
```
```python
>>> hari = {1:'isnin',2:'selasa',3:'rabu'}
>>> print(hari[1])
isnin
```
##  **Jenis Data**

**Jenis Data** _(data type)_ adalah konsep di dalam Python dimana setiap data telah dikelaskan mengikut jenis masing masing.

|   |   |
|---|---|
|**Nama data**|**Jenis Data**|
|teks|str (string)|
|nombor|jenis data: int, float, complex|
|susunan|list, tuple, range|
|pemetaan|dict|
|set|set|
|boolean|bool|
|binary|bytes, bytearray, memoryview|

Bagi mengenalpasti jenis data, kod boleh ditulis menggunakan type() seperti berikut:

```python
>>> nama = 'Jeff'
>>> bilangan = 1, 3, 4, 5
>>> alat_tulis = ['pemadam', 'pensel', 'pembaris']
>>> print(type(nama))
>>> print(type(bilangan))
>>> print(type(alat_tulis))
<_class_ 'str'>
<_class_ 'tuple'>
<_class_ 'list'>
```
· Menetapkan _Data Type_  yang Spesifik

Adakalanya, jenis data yang kita tulis akan dibaca dengan jenis data berlainan daripada apa yang kita mahukan. Justeru itu, Python menyediakan cara untuk menetapkan secara spesifik data tersebut menggunakan arahan tertentu seperti berikut:

|   |   |
|---|---|
|_Data Type_|Contoh|
|**str ()**|**x = str ('hello dunia!')**|
|**int ()**|**x = int (30)**|
|**float ()**|**x = float (0.124)**|
|**complex()**|**x = complex (2j)**|
|**list()**|**x = list (('pisang', 'manggis', 'rambutan'))**|
|**tuple ()**|**x = tuple (('pisang', 'manggis', 'rambutan'))**|
|**dict()**|**x = dict (nama = 'Mat', umur = '10')**|
|**range()**|**x = range (78)**|

Dengan menetapkan _Data Type_  metod, anda dapat menukar jenis data asal kepada yang dikehendaki kepada Python. 

  

##  **Komen**

Adakalanya apabila kita menulis kod, kita mahu meletakkan nota ataupun komen pada kod anda supaya anda dapat mengingati apakah yang dimakssudkan oleh kod tersebut.

Untuk menyatakan bahawa baris kod tersebut adalah komen, anda boleh meletakkan awalan tanda pagar (#) pada sebelah kod dengan. Komen ini **tidak akan dibaca** oleh Python sekaligus  tidak mengganggu proses membaca kod.

```python
>>> #senarai barang
>>> x = 'fish'*
>>> y = 'meat'
>>> print(x)
>>> print(y)
fish
meat
```
Perhatikan yang **#senarai barang**, **#barang1**, dan  **#barang2** tidak dibaca oleh Python dan _output_ yang terhasil masih sama tanpa perubahan.

Praktis meletakkan komen membantu anda menulis kod secara sistematik dengan pembahagian kod mengikut komen yang anda telah tetapkan. Menggunakan komen juga, anda boleh mengingati semula tentang apakah konteks kod anda dengan ayat yang anda sendiri fahami.

Bukan itu sahaja, komen membantu gerak kerja yang melibatkan lebih daripada seorang pengaturcara untuk memahami konteks kod masing-masing.

##  **help ()**

Dalam Python, ia menyediakan satu metod yang membolehkan kita meminta Python untuk menerangkan kata kunci Python tersebut. Contoh,
```python
>>> help('print')
Help on built-in function print in module builtins:
print(...)
    print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=**False**)
    Prints the values to a stream, or to sys.stdout by default.
    Optional keyword arguments:
    file:  a file-like _object_ (stream); defaults to the current sys.stdout.
    sep:   string inserted between values, default a space.
    end:   string appended after the last value, default a newline.
    flush: whether to forcibly flush the stream.
```
Jadi, jika anda kebuntuan atau mahukan pemahaman dengan lebih mendalam mengenai sesuatu metod atau fungsi, gunakan _help_ untuk mendapatkan penerangan tersebut.

##  **Tarikh**

· **Datetime**

Python telah menyediakan satu modul dimana pengaturcara dapat menggunakan modul tersebut untuk menyatakan masa dan jam pada ketika itu.  
```python
>>> import datetime as dt
>>> x = dt.datetime.now()
>>> print(x)
2021-09-12 11:20:18.162425
```


_Datetime_ juga membenarkan pengaturcara untuk mencipta tarikh sendiri seperti berikut;
```python
>>> import datetime as dt
>>> x = dt.datetime(2021, 9, 12)
>>> print(x)
>>> print(x.year)
2021-09-12
2021
```

Selain daripada itu, pengaturcara juga boleh mengkhususkan _output_  tertentu dengan menggunakan metod **strftime( )**.
```python
**>>> import datetime as dt
**>>> x = dt.datetime.now()
**>>> print(x.strftime('%A'))
**>>> print(x.strftime('%a'))
Sunday
Sun
```
“%A” dan “%a” adalah format kod yang membawa maksud hari minggu untuk versi panjang dan hari minggu untuk versi pendek. Terdapat pelbagai lagi format kod yang ada. Anda boleh merujuknya di laman sesawang di bawah:

[https://www.w3schools.com/python/python_datetime.asp](https://www.w3schools.com/python/python_datetime.asp)

  

##  **Logik Boolean**

Logik secara asasnya bermaksud mengenal pasti samada sesuatu fakta itu adalah benar ataupun salah. Di dalam kehidupan seharian manusia, kita selalu berhadapan dengan keadaan menentukan sama ada sesuatu itu benar atau salah. Penilaian manusia biasanya berdasarkan pengetahuan, pengalaman dan tidak lupa juga faktor luar yang mempengaruhi.

Di dalam Python, terdapat logik yang dinamakan sebagai Python Boolean. Boolean yang terdapat di dalam Python menggunakan kata kunci **True** dan **False**. Boolean adalah sejenis _built-in data type_. Maka ia tidak perlu diimport daripada luar secara manual.

Sebagai contoh, 14 > 2 adalah **True**, manakala 1 == 5 adalah **False**. Kita sendiri boleh memikirkan logika ini. **True** dan **False** adalah katakunci terbina di dalam Python. Oleh sebab itu ia tidak boleh sewenagnya menggunakan ia sebagai _variable_ untuk mewakili sesuatu.

Di dalam Boolean, terdapat kod yang dipanggil Boolean Operator (BO) yang boleh ditulis dalam pembentukan Boolean. BO ini boleh dibahagikan kepadaa 3 kumpulan iaitu, _Logical Operator_, _Identity Operator_ dan _Membership Operator__._

|   |   |
|---|---|
|Jenis operator|Contoh Operator|
|_Logical Operator_<br><br>- digunakan untuk menggabungkan pernyataan bersyarat (_conditional_ )|**and      or      not**|
|_Identity Operator_<br><br>- digunakan untuk membandingkan objek|**is     is not**|
|_Membership Operator_<br><br>- digunakan untuk menguji JIKA terdapat kehadiran urutan dalam objek.|**in     not in**|

Bagi setiap BO terdapat kegunaan yang berbeza.

1.  **and**

**and** akan memberikan _output_  **True** apabila kedua-dua premis yang diberikan adalah betul. Jika salah satu premis adalah salah, _output_ yang diberikan adalah **False**. Jika kedua-dua premis adalah salah maka _output_nya adalah **False**.

Contoh,
```python
>>> x = 8
>>> print (x < 9 and x > 2)
>>> print (x < 9 and x < 7)
>>> print (x < 3 and x < 7)
True
False
False
```
2.  **or**

**or** akan memberikan _output_  **True** jika kedua-dua premis yang diberikan adalah betul DAN jika salah satu daripada premis adalah betul. Manakala jika kedua-dua premis adalah salah, barulah _output_ yang terhasil adalah **False**.

Contoh kod;
```python
>>> x = 7
>>> print ( x > 5 or x > 6)
>>> print ( x > 5 or x > 2)
>>> print ( x > 1 or x > 2)
True
True
False
```

3.   **not**

**not** digunakan bagi mendapatkan _output_ yang songsang daripada _output_ yang sebenar.

Contoh kod;
```python
>>> x = 6
>>> print (not (x <7 and x <10))
False
```
Jika kita dapat membayangkan kod print tersebut tanpa **not**, kita dapat melihat premis yang diberikan adalah **True**. Namun, disebabkan terdapat BO _not_ di awalan, maka _output_ yang terhasil adalah songsang daripada apa yang sepatutnya.

4.    **is**

**is** akan memberikan _output_ **True** jika kedua-dua objek yang dibandingkan adalah sama. Begitu juga sebaliknya jika salah satu atau kedua-duanya berbeza, maka ia akan menghasilkan **False****.**

Contoh kod;

```python
>>> x = 3
>>> y = 3
>>> print (x is y)
True
```

**is not** pula sebalinya. Jika salah satu daripad objek tersebut adalah berbeza, maka _output_ akan menghasilkan **True**.

```python
>>> x = 3
>>> y = 5
>>> print (x is not y)
True
```
5.  **in**

**in** akan memberikan _output_ **True** jika urutan yang mempunyai nilai tertentu terdapat di dalam objek yang dirujuk. Juga sebaliknya jika tiada, maka _ouput_ adalah **False**.

Contoh,
```python
>>> x = ['bunga', 'daun']
>>> print('daun' in x)
True
```
**not in** menyongsangkan apa yang dilakukan oleh in. Jika nilai tersebut tiada dalam urutan (list) objek, maka _output_ adalah **True**. Begitu juga sebaliknya.

```python
>>> x = ['bunga', 'daun']
>>> print('kayu' not in x)
True

```
  

##  **Conditional Statement**

Kita mulakan subtopik ini dengan sebuah analogi. Pada sebuah hujung minggu, ibu anda meminta anda untuk pegi ke pasar raya bagi membeli barang dapur. Beliau meminta anda untuk membeli ikan bawal, tetapi beserta syarat tertentu. Syaratnya adalah;

1. Anda perlu membeli sebanyak 5 ekor.

2. Berat seekor ikan tidak melebihi 2 kilogram.

3. Jenis ikan bawal adalah bawal emas.

Anda perlu mematuhi semua syarat ini kerana ibu anda sangat cerewet dalam memasak. Keadaan dimana anda perlu mematuhi syarat-syarat adalah suatu kebiasaan dalam kehidupan seharian. Contoh lain, syarat-syarat kemasukan sekolah, syarat-syarat pertandingan

Dalam bidang pengaturcaraan, syarat yang diberi oleh anda dikenali sebagai **_conditional statement_****.**

Dalam sebuah pembentukan _condition_ terdapat beberapa komponen yang digunakan iaitu, **if****,** **elif****,** dan **else**. Terdapat sebab mengapa penulis menulis ia mengikut susunan begini. Lihat contoh kod dibawah;

```python
>>> x = 10
>>> if x >10:
>>>	print('x is bigger than 10')
>>> elif x = = 10:**
>>>	print('x is equal to 10.')
>>> elif x < 10:
>>> 	print('x is less than 10')

x is equal to 10.
```

· **if** ditulis hanya untuk syarat pertama. Syarat pertama dalam kod diatas adalah nilai x perlu melebihi 10. Untuk syarat seterusnya, kata kunci **elif** akan digunakan sebagai awalan syarat tersebut. Syarat kedua dan ketiga adalah nilai x perlu bersamaan dengan 10 ataupun nilai x adalah kurang daripada 10.

Bagaimana pula dengan **else**?

· **else** digunakan untuk syarat akhir code tanpa apa-apa syarat yang mengikatnya, dimana bererti, selain daripada syarat-syarat yang dikenakan di atasnya, akan terpakai padanya.

Contoh kod;
```python
>>> x = 6
>>> if x >10:
>>> 	print('x is bigger than 10')
>>> elif x = = 10:*
>>> 	print('x is equal to 10.')*
>>> else:**
>>>	print('x is less than 10')
x is less than 10.
```
Dengan hanya menggunakan arahan mudah ini, anda mampu memanipulasi kod supaya mengikuti arahan yang kita kehendaki secara automatik. Subtopik ini yang menjadi asas kepada kewujudan mesin pembelajaran apabila kod ini seolah-olah mampu ‘berfikir’ lalu membuat keputusan.

  

##  **F****unction**

Setelah mengetahui asas kepada penulisan kod, sekarang anda akan mempelajari bagaimana rangkumkan keseluruhan kod tersebut untuk diletakkan di dalam sebuah  struktur yang dikenali sebagai _function_.

 Fungsi akan dimulakan dengan **def** , kemudian diikuti dengan nama fungsi tersebut, disusuli dengan kurungan yang diisi dengan _argument_ dan diakhiri dengan titik dua bertindih. 

**def** ***func_name** **( *argument)****:**

**return** **_something_**

Maklumat dapat dipindahkan ke dalam fungsi melalui _argument_.

Contoh _function_:

```python
>>> def kucing(nama):
>>> 	print ('Nama kucing penulis' + ' ' + nama):
>>> kucing('Oyen')
Nama kucing penulis Oyen
```
Jika diperhatikan, maklumat **'Oyen'** telah dipindahkan ke dalam _argument_ **nama** pada fungsi **def** **kucing** dan _output_ yang terhasil bergabung bersama string “**Nama kucing** **penulis**'.

Bagi menghasilkan output, fungsi definisi akan menggunakan kata-kunci `return` yang merujuk kepada hasil akhir fungsi tersebut.

Contoh,

```python
>>> def y(x):
>>> 	 return 10 + x
>>> y(7)
17
```
Bilangan _*argument_ adalah tidak terbatas. Bergantung kepada fungsi apa yang ingin ditulis oleh pengaturcara.

```python
>>> def add_this_value(val_1, val_2, val_3):
>>> 	 return val_1 + val_2 + val_3
>>> add_this_value(10, 20, 30)
60
```
_Function_  juga boleh digunapakai dalam _function_ yang lain. Misalnya;

```python
>>> def return_max_val(number_list):
>>> 	max = 0
>>> 	for val in number_list:
>>> 		if val > max:
>>> 			max = val
>>> max_value = return_max_val([1,2,3])
>>> add_this_value(max_value, 20, 30)
53
```


Jika diperhatikan dalam _function_ return_max_val _, function_ ini akan mengambil _list_ nombor sebagai argumen. Daripada argumen tersebut, akan digunakan pada _for-loop_ yang mana algoritma ini akan mengenalpasti nombor yang besar daripada nombor sebelumnya dan nilai tersebut akan disimpan pada _variable_ max. _Function_ ini akan memhasilkan hasil akhir nombor terbesar dalam _list_  nombor tadi, dan nilai tersebut akan digunakan dalam _function_ add_this_value untuk proses tambah.

_Function_ adalah seperti sebuah kilang roti. Terdapat pelbagai perkara yang berlaku dalam proses ini. Proses-proses yang berlaku dalam kilang ini adalah seperti baris-baris kod yang melakukan sesuatu dalam _function_ dan roti tersebut adalah hasil akhir yang akan di-_return_-kan pada akhir _function_ tersebut.

  

###  **input** 

Dalam Python menyediakan satu fungsi yang dinamakan input(). Input mengambil maklumat daripada _user_ untuk disimpan dalam _variable_ tertentu.

Kod boleh ditulis seperti berikut;

```python
>>> x = input ('Insert your number here:')
Insert your number here:
```
Untuk menggunakan **input()**, anda perlu meletakkan _prompt_; sebuah arahan untuk diberikan kepada pengguna supaya memasukkan maklumat yang sepatutnya ke dalam program. Di dalam kod di atas, _prompt_ yang digunakan adalah 'Insert your number here:'.

_Output prompt_ seperti di atas akan terhasil dimana program akan meminta _input_ apa ,yang kita mahukan. Selepas menulis apa _input,_  tekan _Enter_. Dan kod akan berjalan seperti biasa.

Penggunaan input() akan menghasilkan kod yang interaktif.

  

##  Loop

Dalam pengaturcaraan, _loop_ (_loop_) adalah sebuah konsep dimana beberapa siri perbuatan yang sama yang dilakukan berulang kali.

Sebagai contoh proses untuk memasak sebiji burger.

1. Mulakan dengan mengambil 2 keping roti.

2. Panaskan minyak atas pan.

3. Ambil sekeping daging dan masak.

4. Usai masak, letak daging atas roti tadi.

5. Potong beberapa hirisan timun dan letakkan atas daging.

6. Picit sos dan mayonis keatas timun.

7. Tutup sayur tadi dengan sekeping roti.

8. Siap.

Diatas ini adalah satu proses penuh untuk mencipta seketul burger. Untuk mencipta burger yang seterusnya, maka kita harus melalui proses yang sama.  Seandainya terdapat 100 burger yang anda ingin jual, maka anda akan buat 100 kali _loop_ untuk menyiapkan kesemua 100 burger tersebut.

Kerja yang sama dan berulang ini dipanggil sebagai _iteration_ _(_iteration). Disebabkan proses manual memasak diatas sangat membosankan kerana berulang,  pengaturcara yang bijak hanya perlu mencipta sebuah _loop_ untuk menyiapkan kesemua 100 burger tersebut.

Kod yang mengandungi arahan untuk menjalankan kerja yang sama yang berulang tersebut dipanggil sebagai _loop_.

Selain daripada itu, anda juga boleh meletakkan _conditionl statement_ kepada Python seperti, apabila kesemua 100 burger telah siap, sila berhenti (_break_).

Di dalam Python, terdapat dua jenis _loop_ iaitu: 

· for _loop_

· while _loop_

Kedua-duanya mempunyai objektif yang sama iaitu untuk mengautomatikkan beberapa siri perbuatan, tetapi terdapat sedikit perbezaan.

###  **For** **loop**

_For loop_ digunakan untuk menjalankan _iteration_ pada struktur data yang _iterable_ iaitu _list, tuple,_ dan _dictionary_. Untuk menggunakan _for_ _loop_, kod seperti berikut akan ditulis iaitu,
```python
for data in y:
	# do_something_1
	# do_something_2
```

Contoh kodnya,
```python
>>> y = [1, 2, 3, 4, 5]
>>> for data in y:
>>> 	print(data)
1
2
3
4
5
```

Apa yang berada dibawah _for_ haruslah diperenggankan (_indent_) bagi menunjukkan arahan tersebut berada dibawah lingkungan _loop_ yang dicipta. data mewakili nilai-nilai yang terkandung di dalam list bernama y.

Bagi menambah syarat ke dalam kod, ia boleh ditulis dengan,

```python
>>> y = [1,2,3,4,5,6]
>>> for data in y:
>>> 	if data < 4:
>>> 	print(data)
1
2
3
```
_loop_ membaca senarai nombor yang berada dalam _list_ y dan jika terdapat nilai yang kurang daripada 4, maka hanya nilai tersebut yang akan dikeluarkan _output_. Jika nilai lebih daripada 4, ini memberhentikan proses _loop_.

Selain daripada itu, terdapat satu lagi cara bagi memberhentikan proses _loop_ iaitu menggukan **break**.

```python
>>> y = [1,2,3,4,5,6]
>>> for data in y:
>>>     print(data)
>>>     if data > 4:
>>>        break
1
2
3
4
5
```
_loop_ akan membaca senarai nilai dalam _list_-y. Jika _iteration_ menemui nilai yang lebih daripada 4 (iaitu 5 dalam senarai ini), maka _loop_ akan berhenti. Tetapi 5 tetap dihasilkan kerana nilai 5 adalah kayu penanda di dalam kod supaya ia diberhentikan. Dalam kod ini, _iteration_ setelah menjumpai 5, maka dengan itu, _loop_ harus diberhentikan.

Tidak hanya memberhentikan, kita juga boleh menyambung proses _loop_ dengan menggunakan kata kunci **continue**.

Contoh;
```python
>>> nombor = [1,2,3,4,5]
>>> for x in nombor:
>>>   if x == 3:
>>>     continue
>>> print(x)
1
2
4
```
Apabila _iteration_ menemui nilai 3, maka _loop_ diberitahu supaya meneruskan proses _iteration_ hingga ke data terakhir iaitu 5. Nombor 3 tidak terhasil kerana 3 adalah kayu ukur penanda supaya meneruskan _iteration_. Cara ini sangat berguna jika kita ingin memeriksa kewujudan nombor atau string di dalam sebuah list itu. Jika ia wujud, maka teruskan. Jika tidak wujud, iteration tidak akan diteruskan.

Contoh _loop_ **for** yang menggunakan **dictionary**:
```python
>>> data = {'nama': 'Jack', 'hobi' : 'badminton'}
>>> for k,v in data.items():
>>> 	print(k,v)
nama Ammar
hobi badminton
```
Kod di atas menggunakan data dalam bentuk **dictionary**. Dalam _loop_ for, kod ini telah menggunakan dua _variable_ bagi menyimpan elemen-elemen di dalam dictionary iaitu **k** dan **v**.

Data pula telah menggunakan **.items()** dimana salah satu metod Dictionary yang mana berfungsi untuk memasangkan key dan value di dalam dictionary. Apa yang ingin disampaikan adalah, anda boleh menggunakan lebih daripada 1 _variable_ di dalam _loop_ for bagi menjalankan iteration.

####  **range ( )**

Selain daripad menggunakan list untuk menyenaraikan data, **range()** juga boleh digunakan di dalam _for loop_. **range()** berfungsi bagi menyenaraikan **nombor** dengan julat tertentu.

· **range (mula, akhir, nilai anjak)**

o **mula : nilai mula. Nilai lalai adalah 0.**

o **akhir: nilai henti. Tidak termasuk**

o **nilai anjak: beza daripada satu nilai dan nilai seterusnya.**

Contoh;

Nombor meningkat:

```python
>>> for data in range(1, 4, 1):
>>> 	print(data)
1
2
3
```
Nombor yang terhasil adalah 1, 2 dan 3. Nombor 4 tidak termasuk seperti yang telah dinyatakan diatas.

Nombor menurun:



Tanpa meletakkan nilai akhir dan nilai anjak:

```python
>>> for data in range(5, 1, -1):
>>> 	print(data)
5
4
3
```

| **Indeks** | **Nilai output** |
| ---------- | ---------------- |
| 1          | 0                |
| 2          | 1                |
| 3          | 2                |
| 4          | 3                |

####  **enumerate ( )**

Terdapat sebuah fungsi di yang dapat membantu kod mengira jumlah _iteration_ yang telah dilakukan oleh sesebuah _loop_. Fungsi tersebut adalah **enumerate()**.

Mari lihat contoh penggunaan **enumerate()**.

```python
>>> name = ['Azizul', 'Esma', 'Faiq', 'Aqhmal']
>>> for data in enumerate(name):
>>>    print(data)
(0, 'Azizul')
(1, 'Esma')
(2, 'Faiq')
(3, 'Aqhmal')
```

Seperti yang anda dapat lihat pada _output_ data di atas, pada setiap elemen di dalam _list_ **name**, terdapat nilai indeks yang bersebelahan dengannya yang mengira bilangan _iteration_ yang telah dilakukan.

###  **While** **loop**

_While loop_ adalah sebuah _loop_ yang bertindak menjalankan kod secara berterusan dan berulang selagi mana kod itu menepati syarat yang telah ditetapkan.

_While loop_  yang biasa terdiri daripada 3 komponen asas iaitu:

1. Nilai permulaan

2. Syarat

3. _Increment value_

Mari lihat contoh kod,

```python
>>> k = 1
>>> while k < 5:
>>>     print(k)
>>>    k += 1

1
2
3
4
5
```

Nilai k adalah **nilai permulaan** supaya _loop_ dapat dijalankan. Setelah itu, _loop_ diteruskan dengan **syarat**, iaitu selagi mana nilai k  kurang daripada 5, maka _loop_ akan diteruskan. Pada _output_ pertama iaitu 1, nilai k yang baharu ini akan masuk ke dalam persamaan k += 1  yang sama erti dengan k = k + 1.

Nilai 1 akan masuk pada nilai k. Maka, nilai k yang baru terhasil iaitu k bersamaan dengan 2. Nilai 2 adalah kurang daripada 5, maka _loop_ akan berjalan lagi. Proses ini berulang sampailah nilai k sama dengan 5, maka proses lingakaran akan berhenti serta merta.

Seperti juga _for loop_, dalam _while loop_ juga menggunakan _break_ dan _continue_ dengan tujuan yang sama iaitu memutuskan _loop_ dan menyambung _loop_. Contoh,

```python
>>> k = 1
>>> while k < 7:
>>> print(i)
>>> if (k == 4):
>>>      break
>>>    k += 1
1
2
3
4
```
Apabila _loop_ bertemu dengan nilai k baharu yang bernilai 4, maka _loop_ akan terus diberhentikan serta merta.


_Loop_ akan melangkau nilai 4 apabila _loop_ sampai ke nilai k baharu 4 dan meneruskan _loop_ hingga ke nilai 7 dan berhenti.

###  **While** **True**

Dalam _loop_  yang sebelum ini, kita dapat lihat dimana _loop_ tersebut mempunyai had tertentu sebelum ia berhenti pada suatu keadaan yang telah ditetapkan.

Namun, kita sebenarnya boleh mencipta _loop_ yang berterusan selama-lamanya tanpa ada keadaan yang dapat memberhentikannya.

Dalam Python, kita akan gunakan **while True** untuk mencipta _loop_ ini.  

```python
>>> x = 0
>>> while True:
>>>     x = x + 1
>>>     print(x)
1
2
3
4
5
6
7
8
```
Dalam kod diatas, output akan terhasil selama-lamanya tanpa henti (kecuali anda memberhentikannya) dengan menggunakan  **while True.**

Walaubagaimanapun, anda masih lagi boleh meletakkan keadaan untuk memberhentikan _loop_ ini seperti yang telah kita pelajari sebelum ini dengan menggunakan katakunci **break****.**

```python
>>> x = 0
>>> while True:
>>>     x = x + 1
>>>     print(x)
>>>     if x == 5:
>>>         break
1
2
3
4
5
```
_Loop_ diatas berhenti apabila mencapai nilai 5.

###  **Carta Alir** 

Di dalam memahami gerak kerja sebuah kod, terdapat satu cara yang dipanggil Carta Alir (_flow chart_). Carta Alir adalah sebuah penerangan visual menggunakan bentuk dan anak panah bagi menerangkan apa yang berlaku dalam sesebuah kod. Secara amnya, bentuk dan kegunaan bentuk itu dapat difahami seperti berikut.

-- gambar 

 Penggunaan Carta Alir sangat membantu perjalanan proses kod pada peringkat awal. Lihat contoh Carta Alir dengan kod dibawa:

```python
>>> x = 5
>>> if x > 5:
>>> 	print('x is bigger than 5')
>>> elif x == 5'
>>> 	print('x equal to 5')
X is equal to 5
```
-- gambar 

Melalui Carta Alir di atas, kita dapat melihat apa yang sedang berlaku di dalam kod yang sedang ditulis. Dimana terdapat pernyataaan _if_ dan _elif_ yang telah menyebabkan aliran terpecah kepada dua yang memberi syarat kepada input yang diberikan sebelum menuju kepada arahan seterusnya.

Pada laluan x == 5, alirannya adalah **True** maka arahan akan diteruskan melalui aliran ini, manakala pada laluan x > 5, alirannya adalah **False**, maka laluan ini tidak akan digunakan oleh Python.

Carta Alir sangat berguna bagi membayangkan situasi kod lebih lebih lagi jika kod tersebut lebih rumit seperti memunyai pernyataan _if_ di dalam pernyataan _if_, mempunyai fungsi di dalam fungsi, mempunyai pernyataan _if_ di dalam _loop_ dan sebagainya.

Jika anda buntu semasa menulis kod, berundur selangkah ke belakang dan lukis Carta Alir bagi menyusun semula struktur idea dalam minda.

Praktis ini sangat baik dan lama kelamaan, kita dapat membina sendiri Carta Alir di dalam minda sekalipun tanpa melukis di atas kertas.

###  **Nested** **loop** 

_Nested_ _loop_  adalah sebuah kod _loop_ yang berada di dalam sebuah _loop_ yang lain. Perkataan _nested_ (sarang) digunakan kerana ia seperti seekor burung yang sedang duduk di dalam sebuah sarang yang mengelilinginya. Struktur _l__oop_ ini boleh wujud samada _loop_ luarnya adalah _loop_-for di dalamnya _loop_-while, ataupun sebaliknya, ataupun kedua-duanya adalah lingakaran yang sama.

_Nested loop_ biasanya digunakan dalam struktur data berbilang dimensi.

-- gambar

Dalam _nested loop_, terdapat 2 jenis _loop_ iaitu _loop_ luar dan _loop_ dalam. _L__oop_ luar akan dilaksanakan terlebih dahulu, tetapi sembelum _loop_ luar berjaya dilaksanakan dengan sempurna, _loop_ dalam akan dilaksanakan barulah _loop_ luar akan sempurna.

Mari kita lihat contoh.

```python
>>> import time

>>> x = range(3)
>>> for i in x:
>>>    time.sleep(2)
>>>    print("loop berlangsung...")
>>>    time.sleep(2)
>>>    for j in x:
>>>        print(i, j)
>>>    time.sleep(2)
>>>    print("loop sempurna")
Output:
loop berlangsung...
0 0
0 1
0 2
loop sempurna
loop berlangsung...
1 0
1 1
1 2
loop sempurna
loop berlangsung...
2 0
2 1
2 2
loop sempurna
```
Apa yang terjadi dalam _loop_ ini? Mari kita pergi satu persatu.

· Pada baris 3, anda telah menetapkan _variable_ yang menyimpan nilai 0, 1, 2 yang dibentuk menggunakan fungsi **range().**

· Kemudian kod mencipta sebuah _loop_ tersarang yang terdiri daripada _loop_ luar dan _loop_ dalam.

· _L__oop_ luar akan mengalami _iteration_ terlebih dahulu dimana 0, 1, dan 2 akan dihasilkan. Sintaks "_loop_ berlangsung..." akan dihasilkan. Tetapi _iteration_ ini tidak sempurna selagi mana _loop_ dalam tidak menyempurnakan _loop__-_nya terlebih dahulu.

· Anda dapat lihat terdapat pasangan nombor yang terhasil, dimana nombor kiri adalah hasil _loop_ luar (_variable-i)_, nombor kanan adalah hasil _loop_ dalam (_variable-j)_.

· Maka, pada setiap kali _loop_ luar dijalankan, _loop_ dalam akan mengambil nilai tersebut dan menjalankan proses _loop_ pula padanya. Buktinya dapat dilihat pada _output_ apabila nilai 0 terhasil sebanyak tiga kali bersama pasangan nombor 0, 1, dan 2.

· Selepas itu, barulah sintaks "_loop_ sempurna" yang membawa maksud _loop_ untuk nilai pertama untuk _loop_ luar sudah sempurna.

· Kemudian nilai yang seterusnya iaitu 1 pula berlangsung dengan proses  yang sama.

Dibawah penulis sertakan gambaran carta alir bagaimana kod diatas berfungsi; (abaikan time.sleep() kerana ia cuma bertujuan untuk melambatkan proses sintaks bagi memperlihatkan proses _loop_. Anda boleh cuba kod ini pada IDE anda dan lihat hasilnya).

-- gambar

##  Perenggan

· Indentation

Anda dapat perhatikan bahawa apabila bermulanya masuk tajuk _Function_ dan _Condition_, terdapat satu cara penulisan yang bermula dengan perenggan atau dikenali sebagai _indentation__._

Terdapat dua keadaan dimana _indentation_ digunapakai iaitu semasa menggunakan _Function_ def dan semasa membuat condition. Contoh indentation dalam _Function_,
```python

def kucing(nama):
<-->print ('Nama kucing penulis' + ' ' +nama):
```

`<-->` menunjukkan dibawah def perlu mengenakan perenggan. (anak panah cuma ingin merujuk terdapat perenggan di bahagian tersebut dan bukannya perlu menulis anak panah tersebut.)

Sama juga seperti condition,

```python
>>> if x > 2:
>>> <--> print('x bigger than 2.')
```
_Nest_ juga ada berlaku di dalam for loop dan while loop,
```python
>>> car = ['Wira', 'Perodua', 'Saga']
>>> for data in car:
>>> <--> print(data)
Wira
Perodua
Saga
```
Contoh while loop

```python
>>> i = 0
>>> while True:
>>> <--> print ('Counting is processed...')
>>> <--> if i == 5:
>>> <-----> break
>>> <--> i = i + 1
>>> print (i)
Counting is processed...
Counting is processed...
Counting is processed...
Counting is processed...
Counting is processed...
Counting is processed...
5
```
_Indentation_ sangat penting dalam pembinaan sebuah kod. Ini kerana ia menetukan arahan tersebut di bawah blok yang spesifik.

Dapat diperhatikan di dalam kod while loop, persamaan i = i + 1 berada di luar kod if dimana ini bermaksud persamaan tersebut tertakluk pada while loop. Untuk penjelasan lebih lanjut di dalam gambar dibawah,

-- gambar

Mengikut gambarajah di atas, kod bermula dengan while **True**, dimana ini memberi arahan kepada Python untuk terus menerus menjalankan kod dan menghasilkan _string_ “Counting is processed” pada berikutnya. Kod digerakkan menggunakan persamaan **i = i + 1** dan diberikan sebuah kondisi iaitu jika i bersamaan dengan 5, makan kod akan diberhentikan dengan arahan break. Maka terhasillah _output_ yang ditunjukkan di atas.

##  **Library**

Secara amnya, _library_ adalah satu himpunan kod yang dikumpulkan di dalam satu ruang bernama _package__._ Setiap _library_ mempunyai kegunaan tertentu seperti perkiraan Matermaik, membuat graf, mengumpul data dan sebagainya. _Package_ pula terdiri daripada himpunan _module_ iaitu kod-kod yang menjalankan fungsi tertentu.

Berikut adalah contoh _library_ yang seringkali digunakan untuk perkiraan Matematik dan memanipulasi data. Antaranya;

· math

· numPy

· Pandas

· Seaborn

· Matplotlib

Selain daripada itu, terdapat juga _library_ yang digunakan untuk proces _web scrapping_ iaitu proses mengeluarkan maklumat daripada laman web. _Library_ yang digunakan ialah:

· Selenium

· Beautifulsoup

###  **numPy**

Numpy atau Number Python adalah sebuah _library_ yang menyediakan fungsi berkaitan dengan matematik dan juga matriks.

Dengan menggunakan numPy, anda boleh mencipta sebuah matriks (_array_) dan melakukan operasi kepadanya.  Mari kita lihat contoh penggunaan numPy.

```python
import numpy as np

>>> a = np.array([[1,2,4], 
                [3,5,7], 
                [3,4,6]])
>>> b = np.array([[2,5,9], 
                 [-1,8,9], 
                 [2,4,3]])
>>> c = b - a
>>> print(c)
[[ 1  3  5]

 [-4  3  2]

 [-1  0 -3]]
```
Dalam kod di atas, _array_ telah dicipta dengan kod np.array dan ditulis di dalamnya matriks dalam bentuk list. Jika dapat dilihat, ini adalaha matriks 3 X 3, dengan 3 lajur dan 3 baris.

Seterusnya, operasi penolakan dilakukan dan anda dapat lihat ouput kepada kod ini adalah hasil tolak _array_ A dan _array_ B.

Anda juga boleh menyeru nombor, lajur dan baris di dalam _array_ dengan menggunakan index koordinat nombor tersebut.

```python
>>> print(c[0,1])
>>> print(c[0])
>>> print(c[0, :])
>>> print(c[:, 0])
3
[ 1  3  5]
[ 1  3  5]
[ 1  -4  -1]
```
Pada kod pertama, c[0,1] bermakna nilai pada lajur 0 iaitu lajur pertama (ingat semula dalam topik list dimana indeks bermula dari 0) dan juga baris 1 dimana baris kedua.

###  **dir( )**

Bagi setiap _library_, terdapat pelbagai modul dan fungsi yang telah tersedia untuk digunakan oleh pengaturcara. Modul dan fungsi ini boleh disemak dengan menggunakan fungsi **dir ()** dengan seperti contoh berikut,

```python
>>> import datetime as dt
>>> dir (dt)
['MAXYEAR','MINYEAR','__builtins__','__cached__','__doc__','__file__','__loader__','__name__','__package__','__spec__','date','datetime','datetime_CAPI','sys','time','timedelta','timezone','tzinfo']
```
# **Ralat**

## **Pengenalan**

Ralat atau _error_ adalah sebuah kesalahan yang berlaku semasa dalam penulisan kod yang berpunca daripada pelbagai faktor. Antaranya adalah seperti salah ejaan, tiada perenggan, salah penggunaan metod, kesalahan argumen, jenis data, dan lain-lain lagi.

##  **Nyahpepijat**

Untuk pemula, menulis kod adakalanya menjadi sukar apabila berhadapan dengan ralat. Oleh hal yang demikian, tugas pengaturcara bukan sahaja menulis kod tetapi juga melakukan penyiasatan bagi memeriksa bahagian manakah yang menjadi punca kepada sintaks yang menuju kepada ralat.  Ini yang dipanggil sebagai; nyahpepijat atau _debugging_.

-- gambar 

_Rajah_ _7__: Rama-rama di dalam komputer._

Sejarah perkataan pepijat (bug) ini bermula apabila seorang saintis komputer Amerika, Grace Brewster Murray Hopper yang sedang menggunakan komputer MarkII di Universiti Harvard, apabila rakan sekerjanya menemui rama-rama yang telah tersekat di bahagian dalam komputer yang menyebabkan komputer tersebut gagal daripada untuk berfungsi. Sejak daripada itu, beliau meggunakan pepijat sempena peristiwa tersebut untuk merujuk keadaan dimana kod mengalami masalah dan tidak dapat dilaksanakan.

Dalam Python, kita boleh mengendalikan ralat dengan menggunakan **try****, except** dan **finally.**

##  **Try, Except, Finally** 

Pertamanya kita perlu memahami dahulu maksud **try****, except** dan **finally.**

| Kod         | Maksud                                                                 |
| ----------- | ---------------------------------------------------------------------- |
| **try**     | Menguji baris-baris kod ini sama ada terdapat ralat atau tidak padanya |
| **except**  | Jika ralat berlaku, buat sesuatu.                                      |
| **finally** | Buat sesuatu jika ralat tidak berlaku atau berlaku.                    |

Kita mulakan dengan kod ringkas:
```python
>>> try:
>>>	x = ‘hello world’
>>>	print (x)
>>> except:
>>> 	print ('Please define variable x.')

hello world
```
Output menunjukkan tiada ralat berlaku.

Kita cuba hasilkan ralat dengan tidak meletakkan nilai-x;

```python
>>> try:
		print (x)

>>> except:
		print ('Ralat di sini')

Ralat di sini
```
Output menunjukkan mesej ‘Ralat di sini’ kerana tiada nilai x yang dinyatakan dalam blok kod diatas.

Jika anda inginkan mesej ralat daripada Python, anda boleh tulis seperti berikut;
```python
>>> try:
>>>	print (x)
>>> except Exception as e1:
>>>	print ('Ralat di sini')
>>>	print(e1)

Ralat di sini
name 'x' is not defined
```
Selain daripada ia mengeluarkan mesej yang anda mahukan, ia juga mengeluarkan mesej ralat daripada Python _interpreter_ yang menjalankan kod.

Mari kita kembangkan lagi dengan penggunaan **finally.**

```python
>>> try:
>>> print (x)
>>> except Exception as e1:
>>> print ('Ralat di sini')
>>> print(e1)
>>> finally:
>>> print(‘Kod diatas telah diuji’)

Ralat di sini
name 'x' is not defined
Kod diatas telah diuji
```
Mesej dalam blok **finally** akan terpapar dalam keadaan sama ada ralat berlaku ataupun tidak.