==================
Asas Python
==================

----------------------------
Pengenalan Jupyter Notebook
----------------------------

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

Kita mulakan asas Python dengan memahami konsep *Commander* and *Command*. *Commander* atau komander adalah satu pangkat gelaran yang biasanya diberikan kepada ketua dalam kumpulan askar. Komander akan memberikan arahan (*command*)  kepada askar dibawahnya untuk dilaksanakan.
 
Dalam konteks pengaturcaraan, anda adalah Komander tersebut.

Anda memberi arahan berbentuk barisan kod ke dalam IDE. Kemudian IDE akan membaca kod tersebut dan menjalankannya untuk menghasilkan output.

Untuk memahami dengan mendalam lagi konsep ini dengan cara yang lebih menyeronokkan, penulis mempelawa anda untuk bermain di pantai bersama si penyu! Dalam kod ini, anda akan mempelajari bagaimana ingin menggerakkan penyu. Disebabkan penyu berada di pantai,  pergerakkannya akan menyebabkan kesan pada permukaan dan itu membolehkan anda untuk melukis sesuatu.

Mari kita mulakan permainan ini.

1. Buka **Anaconda Command Prompt** (bukan CMD biasa) dan masukkan kod berikut baris demi baris. Mulakan dengan baris pertama dan klik (*enter*) kemudian kod seterusnya hingga baris akhir.

```python
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

Penyu akan bergerak kehadapan sejauh 100 pixel dan telah berputar 90 darjah ke kiri dari posisi asal. Anda sebagai komander telah memberi arahan bergerak ke hadapan dengan arahan ``t.forward`` (jarak bergerak) dan juga arahan membelok dengan arahan ``t.left`` (sudut membelok).

Penyu akan meninggalkan kesan warna hitam seperti dakwat lukisan apabila dia bergerak.

5. Selain daripada arahan kedepan dan membelok di atas, anda juga boleh mengarahkan penyu dengan arahan berikut;

| **Arahan** | **Maksud** |
| ---- | ---- |
| **t.backward(***jarak***)** | Arahan mengundur |
| **t.right (***sudut***)** | Arahan berputar ke kanan |
| **t.setposition(***koordinat-x, koordinat-y***)** | Arahan menetapkan posisi dalam nilai koordinat. (anda boleh menetapkan mod *grid* pada tempat dimana penyu bermain untuk menentukan posisinya.) |
| **t.home( )** | Arahan untuk kembali semula ke titik mula. |
| **t.penup( )** | Arahan untuk berhenti melukis. (*pen up* adalah seperti mengangkat pen dari kertas) |
| **t.pendown()** | Arahan untuk mula melukis. (*pen down* adalah seperti meletakkan semula pen ke atas kertas.) |

6. Dengan sedikit kekreatifan, hanya dengan menggunakan arahan di atas, anda boleh melukis pelbagai bentuk seperti contoh dibawah!

-- gambar

Ini sedikit kerja penulis berikan buat anda. Cubalah!

Daripada subtopik ini, anda telah memahami bagaimana pengaturcaraan berfungsi dimana terdapat anda sebagai komander yang memberi arahan (*command*) di dalam kod anda. Kod tersebut akan melaksanakan apa yang anda kehendaki dengan syarat kod tersebut haruslah ditulis tanpa kesalahan padanya.

Setelah memahami tentang mekanisma mudah ini, ayuh kita lanjut kepada kod yang bertindak untuk menghasilkan *output* akhir sesebuah kod iaitu, `print ()`.

##  ***Print Function***

· **print ( )**

Kita mulakan asas Pythod dengan sesuatu yang mudah iaitu fungsi **print()****. 

Fungsi **print()** digunakan bagi merumuskan kod yang telah ditulis supaya *output* daripada kod tersebut dapat dihasilkan. *Output* adalah hasil akhir yang terhasil daripada kod yang telah ditulis.

Mari tulis kod pertama anda.

```python
>>> print("Hello dunia!")
Hello dunia!
```

Seperti *printer*, fungsi **print()** mengeluarkan output pada nilai yang diletakkan dalam kurungan fungsi ini.

Anda boleh meletakkan perkataan dan nombor untuk menghasilkan output. Cuba ubah perkataan di atas kepada nombor dan *run* kod tersebut.

##  **Variable**

**Variable** adalah **nama** yang mewakili kepada **sesuatu nilai** dalam sesebuah kod. *Variable* bersifat *case *sensitive* iaitu penggunaan aksara besar atau kecil memberi perbezaan kepada *variable* tersebut.

Misalnya, **fruit** dan **Fruit** adalah sesuatu yang berbeza walaupun maknanya sama. Jadi anda haruslah berhati-hati ketika menulis kerana aksara besar dan kecil memberi makna berbeza kepada Python.

Di bawah adalah contoh *variable*.

>>> kereta = 'wira'
>>> kereta*1 = 'saga'
>>> kereta*2 = 'bezza'
>>> proton = kereta + kereta*1 + kereta*2
>>> print (proton)**

Jika dilihat dalam kod diatas, maklumat nama kereta “wira”, “saga”, dan “bezza” telah disimpan ke dalam *variable* bernama **kereta**, **kereta*1** dan **kereta*2**. Maklumat nama kereta ini telah diapit menggunakan pembuka dan penutup kata (“ “) dan ini mencipta sebuah **string***.*

Di barisan keempat, semua maklumat yang telah disimpan di dalam *variable* disimpan ke dalam *variable* **proton**.

*Variable* juga boleh wujud dalam bentuk persamaan matematik. Contohnya persamaan garis lurus dan formula kecerunan,

**m = (y2 – y1) /(x2 – x1)**

**y = m*x + c**

**m** diatas merujuk kepada formula kecerunan dalam sistem koordinat. Maklumat **m** kemudian disimpan* ke dalam maklumat **y** dimana **y** adalah sebuah persamaan garis lurus.

##  **String**

Di dalam tajuk sebelum ini iaitu *variable*, penulis ada menyebut beberapa kali perkataan *string* dan telah mempunyai definisi iaitu apabila sesuatu perkataan diapit menggunakan pembuka dan penutup kata (“ “). Di dalam Python, *string* boleh dimanipulasi dengan beberapa arahan yang telah ditetapkan. Ia dinamakan sebagai **metod string**.

Contoh,

1. Modifikasi – memanipulasi *string* kepada aksara besar dan kecil.

- variable.upper( )

- variable.lower( )

Contoh kod:

>>> x = 'Nama penulis adalah Ahmad.'
>>> print(x.upper())
>>> print(x.lower())

``NAMA penulis ADALAH AHMAD``

``nama penulis adalah ahmad``

2. Penggabungan

Penggabungan *string* mudah boleh dilakukan dengan dengan hanya menggunakan simbol tambah, **+**.

Contoh kod:

>>> anak*1 = 'Ali'
>>> anak*2 = 'Abu'
>>> anak*mama = anak*1 + '&' + anak*2
>>> print(anak*mama)

``Ali & Abu``

3. Memformat string

· **string*{}.format(argument)**

Memformat string adalah sebuah metod mencipta sebuah templat kosong yang boleh diisi dengan apa-apa maklumat. Bagi menulis stail format, kurungan keriting (*curly bracket*) digunakan sebagai templat tempat kosong. Terdapat 2 cara untuk menulis metod ini.

Cara 1:
```python
>>> bahan*1 = 'ayam'
>>> print('Bahan ayam masak merah adalah {}'.format(bahan*1))
Bahan ayam masak merah adalah ayam
```
Cara 2:
```python
>>> bahan*1 = 'ayam'
>>> print(f'Bahan ayam masak merah adalah** **{bahan*1}')
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

Bagi **float** pula, terdapat perbezaan *output* yang dihasilkan.

Contoh kod:
```python
>>> x = 0.
>>> y = 0.002
>>> print(x+y)
0.10200000000000001
```
Jika diperhatikan daripada *output* kod di atas, jawapan yang terhasil adalah tidak seperti yang diharapkan iaitu, 0.102.  *Output* yang diberikan pula panjang dan mempunyai banyak nilai sifar, diakhir dengan nilai 1.

Python membaca kod ini sebagai **float** atau kita namakan ia sebagai nombor awangan. Walaubagaimanapun, masalah ini boleh diselesaikan dengan fungsi **round()**. Format bagi fungsi **round()** adalah **round(***jawapan akhir, nilai bundar***)**.  Kod diatas boleh diperbaiki kepada berikut;

```python
>>> x = 0.1
>>> y = 0.002
>>> a = round(x + y, 3)
>>> print(a)
0.102
```
##  **Tuple, List, Dictionary, Set**

Pada tajuk yang lepas, kita telah mempelajari berkenaan ***variable*** iaitu satu nama yang digunakan untuk menyimpan maklumat seperti perkataan atau nombor.

Maklumat atau *data* adalah sebuah asas yang sangat penting untuk difahami pada peringkat awal pembelajaran pengaturcaraan. Dalam Python, terdapat beberapa sturktur data yang digunakan yang mempunyai ciri tertentu yang sangat sesuai digunakan dalam banyak keadaan.

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

**List** juga berfungsi sebagai **array**; atau boleh difahami sebagai sebuah bekas atau fail untuk menyimpan maklumat. *List* mempunyai ciri istimewa iaitu maklumat di dalam **List** akan dilabel dengan nombor INDEX (bermula dengan nilai sifar) yang menjadikan penyimpanan maklumat tadi lebih tersusun rapi.

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

Berikut adalah cara untuk mengakses item dalam *list:*
```python
>>> print(minuman[0])
sirap
>>> print(minuman[1])
laici
```
*List* boleh dimanipulasi dengan fungsi tertentu. Antaranya, memasukkan maklumat pada *index* tertentu dengan menggunakan **insert()**, menambah maklumat dengan menggunakan **.append()**, membuang maklumat dengan menggunakan **remove()** ataupun **pop()**, menyusun secara terbalik maklumat dengan **reverse()**, dan lain lain lagi.

Contoh kod;
```python 
>>> minuman.insert(1, 'milo')
>>> print(minuman)
['sirap', 'milo', 'laici', 'kopi', 'teh']
```
```python
>>> minuman.append('limau*ais')
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

Ciri ciri *set* adalah output yang akan terhasil dalam *set* adalah unik dan tidak akan ada yang sama. Jadi jika anda ingin satu set data yang tidak mempunyai pendua, gunakan *set* untuk mencipta output tersebut.

###  **Dictionary** 

*Dictionary* juga menggunakan kurunga keriting seperti *set.* Perbezaannya dengan set (set hanya mempunyai value), **dictionary** menggunakan **key** sebagai rujukan kepada **value**.

Dibawah adalah contoh maklumat dalam bentuk *dictionary*.
```python
>>>test*dict = {"key":"value"}
>>>info = {"name":"Jack", "location":"USA"}
```
*Key* yang sama tidak boleh digunakan secara berulang dalam *dictionary*. Untuk ciri-ciri pula, maklumat boleh ditambah, diubahsuai, dipadam dengan arahan sama seperti yang ada di dalam **list**.
```python
>>> hari = {"hari*1":"isnin","hari*2":'selasa' "hari*3":'rabu'}
>>> print(hari[‘hari*1’])
isnin
```
```python
>>> hari = {1:'isnin',2:'selasa',3:'rabu'}
>>> print(hari[1])
isnin
```
##  **Jenis Data**

**Jenis Data** *(data type)* adalah konsep di dalam Python dimana setiap data telah dikelaskan mengikut jenis masing masing.

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
>>> alat*tulis = ['pemadam', 'pensel', 'pembaris']
>>> print(type(nama))
>>> print(type(bilangan))
>>> print(type(alat*tulis))
<*class* 'str'>
<*class* 'tuple'>
<*class* 'list'>
```
· Menetapkan *Data Type*  yang Spesifik

Adakalanya, jenis data yang kita tulis akan dibaca dengan jenis data berlainan daripada apa yang kita mahukan. Justeru itu, Python menyediakan cara untuk menetapkan secara spesifik data tersebut menggunakan arahan tertentu seperti berikut:

|   |   |
|---|---|
|*Data Type*|Contoh|
|**str ()**|**x = str ('hello dunia!')**|
|**int ()**|**x = int (30)**|
|**float ()**|**x = float (0.124)**|
|**complex()**|**x = complex (2j)**|
|**list()**|**x = list (('pisang', 'manggis', 'rambutan'))**|
|**tuple ()**|**x = tuple (('pisang', 'manggis', 'rambutan'))**|
|**dict()**|**x = dict (nama = 'Mat', umur = '10')**|
|**range()**|**x = range (78)**|

Dengan menetapkan *Data Type*  metod, anda dapat menukar jenis data asal kepada yang dikehendaki kepada Python. 

  

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
Perhatikan yang **#senarai barang**, **#barang1**, dan  **#barang2** tidak dibaca oleh Python dan *output* yang terhasil masih sama tanpa perubahan.

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
    file:  a file-like *object* (stream); defaults to the current sys.stdout.
    sep:   string inserted between values, default a space.
    end:   string appended after the last value, default a newline.
    flush: whether to forcibly flush the stream.
```
Jadi, jika anda kebuntuan atau mahukan pemahaman dengan lebih mendalam mengenai sesuatu metod atau fungsi, gunakan *help* untuk mendapatkan penerangan tersebut.

##  **Tarikh**

· **Datetime**

Python telah menyediakan satu modul dimana pengaturcara dapat menggunakan modul tersebut untuk menyatakan masa dan jam pada ketika itu.  
```python
>>> import datetime as dt
>>> x = dt.datetime.now()
>>> print(x)
2021-09-12 11:20:18.162425
```


*Datetime* juga membenarkan pengaturcara untuk mencipta tarikh sendiri seperti berikut;
```python
>>> import datetime as dt
>>> x = dt.datetime(2021, 9, 12)
>>> print(x)
>>> print(x.year)
2021-09-12
2021
```

Selain daripada itu, pengaturcara juga boleh mengkhususkan *output*  tertentu dengan menggunakan metod **strftime( )**.
```python
**>>> import datetime as dt
**>>> x = dt.datetime.now()
**>>> print(x.strftime('%A'))
**>>> print(x.strftime('%a'))
Sunday
Sun
```
“%A” dan “%a” adalah format kod yang membawa maksud hari minggu untuk versi panjang dan hari minggu untuk versi pendek. Terdapat pelbagai lagi format kod yang ada. Anda boleh merujuknya di laman sesawang di bawah:

[https://www.w3schools.com/python/python*datetime.asp](https://www.w3schools.com/python/python*datetime.asp)

  

##  **Logik Boolean**

Logik secara asasnya bermaksud mengenal pasti samada sesuatu fakta itu adalah benar ataupun salah. Di dalam kehidupan seharian manusia, kita selalu berhadapan dengan keadaan menentukan sama ada sesuatu itu benar atau salah. Penilaian manusia biasanya berdasarkan pengetahuan, pengalaman dan tidak lupa juga faktor luar yang mempengaruhi.

Di dalam Python, terdapat logik yang dinamakan sebagai Python Boolean. Boolean yang terdapat di dalam Python menggunakan kata kunci **True** dan **False**. Boolean adalah sejenis *built-in data type*. Maka ia tidak perlu diimport daripada luar secara manual.

Sebagai contoh, 14 > 2 adalah **True**, manakala 1 == 5 adalah **False**. Kita sendiri boleh memikirkan logika ini. **True** dan **False** adalah katakunci terbina di dalam Python. Oleh sebab itu ia tidak boleh sewenagnya menggunakan ia sebagai *variable* untuk mewakili sesuatu.

Di dalam Boolean, terdapat kod yang dipanggil Boolean Operator (BO) yang boleh ditulis dalam pembentukan Boolean. BO ini boleh dibahagikan kepadaa 3 kumpulan iaitu, *Logical Operator*, *Identity Operator* dan *Membership Operator**.*

|   |   |
|---|---|
|Jenis operator|Contoh Operator|
|*Logical Operator*<br><br>- digunakan untuk menggabungkan pernyataan bersyarat (*conditional* )|**and      or      not**|
|*Identity Operator*<br><br>- digunakan untuk membandingkan objek|**is     is not**|
|*Membership Operator*<br><br>- digunakan untuk menguji JIKA terdapat kehadiran urutan dalam objek.|**in     not in**|

Bagi setiap BO terdapat kegunaan yang berbeza.

1.  **and**

**and** akan memberikan *output*  **True** apabila kedua-dua premis yang diberikan adalah betul. Jika salah satu premis adalah salah, *output* yang diberikan adalah **False**. Jika kedua-dua premis adalah salah maka *output*nya adalah **False**.

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

**or** akan memberikan *output*  **True** jika kedua-dua premis yang diberikan adalah betul DAN jika salah satu daripada premis adalah betul. Manakala jika kedua-dua premis adalah salah, barulah *output* yang terhasil adalah **False**.

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

**not** digunakan bagi mendapatkan *output* yang songsang daripada *output* yang sebenar.

Contoh kod;
```python
>>> x = 6
>>> print (not (x <7 and x <10))
False
```
Jika kita dapat membayangkan kod print tersebut tanpa **not**, kita dapat melihat premis yang diberikan adalah **True**. Namun, disebabkan terdapat BO *not* di awalan, maka *output* yang terhasil adalah songsang daripada apa yang sepatutnya.

4.    **is**

**is** akan memberikan *output* **True** jika kedua-dua objek yang dibandingkan adalah sama. Begitu juga sebaliknya jika salah satu atau kedua-duanya berbeza, maka ia akan menghasilkan **False****.**

Contoh kod;

```python
>>> x = 3
>>> y = 3
>>> print (x is y)
True
```

**is not** pula sebalinya. Jika salah satu daripad objek tersebut adalah berbeza, maka *output* akan menghasilkan **True**.

```python
>>> x = 3
>>> y = 5
>>> print (x is not y)
True
```
5.  **in**

**in** akan memberikan *output* **True** jika urutan yang mempunyai nilai tertentu terdapat di dalam objek yang dirujuk. Juga sebaliknya jika tiada, maka *ouput* adalah **False**.

Contoh,
```python
>>> x = ['bunga', 'daun']
>>> print('daun' in x)
True
```
**not in** menyongsangkan apa yang dilakukan oleh in. Jika nilai tersebut tiada dalam urutan (list) objek, maka *output* adalah **True**. Begitu juga sebaliknya.

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

Dalam bidang pengaturcaraan, syarat yang diberi oleh anda dikenali sebagai ***conditional statement*****.**

Dalam sebuah pembentukan *condition* terdapat beberapa komponen yang digunakan iaitu, **if****,** **elif****,** dan **else**. Terdapat sebab mengapa penulis menulis ia mengikut susunan begini. Lihat contoh kod dibawah;

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

Setelah mengetahui asas kepada penulisan kod, sekarang anda akan mempelajari bagaimana rangkumkan keseluruhan kod tersebut untuk diletakkan di dalam sebuah  struktur yang dikenali sebagai *function*.

 Fungsi akan dimulakan dengan **def** , kemudian diikuti dengan nama fungsi tersebut, disusuli dengan kurungan yang diisi dengan *argument* dan diakhiri dengan titik dua bertindih. 

**def** ***func*name** **( *argument)****:**

**return** ***something***

Maklumat dapat dipindahkan ke dalam fungsi melalui *argument*.

Contoh *function*:

```python
>>> def kucing(nama):
>>> 	print ('Nama kucing penulis' + ' ' + nama):
>>> kucing('Oyen')
Nama kucing penulis Oyen
```
Jika diperhatikan, maklumat **'Oyen'** telah dipindahkan ke dalam *argument* **nama** pada fungsi **def** **kucing** dan *output* yang terhasil bergabung bersama string “**Nama kucing** **penulis**'.

Bagi menghasilkan output, fungsi definisi akan menggunakan kata-kunci `return` yang merujuk kepada hasil akhir fungsi tersebut.

Contoh,

```python
>>> def y(x):
>>> 	 return 10 + x
>>> y(7)
17
```
Bilangan **argument* adalah tidak terbatas. Bergantung kepada fungsi apa yang ingin ditulis oleh pengaturcara.

```python
>>> def add*this*value(val*1, val*2, val*3):
>>> 	 return val*1 + val*2 + val*3
>>> add*this*value(10, 20, 30)
60
```
*Function*  juga boleh digunapakai dalam *function* yang lain. Misalnya;

```python
>>> def return*max*val(number*list):
>>> 	max = 0
>>> 	for val in number*list:
>>> 		if val > max:
>>> 			max = val
>>> max*value = return*max*val([1,2,3])
>>> add*this*value(max*value, 20, 30)
53
```


Jika diperhatikan dalam *function* return*max*val *, function* ini akan mengambil *list* nombor sebagai argumen. Daripada argumen tersebut, akan digunakan pada *for-loop* yang mana algoritma ini akan mengenalpasti nombor yang besar daripada nombor sebelumnya dan nilai tersebut akan disimpan pada *variable* max. *Function* ini akan memhasilkan hasil akhir nombor terbesar dalam *list*  nombor tadi, dan nilai tersebut akan digunakan dalam *function* add*this*value untuk proses tambah.

*Function* adalah seperti sebuah kilang roti. Terdapat pelbagai perkara yang berlaku dalam proses ini. Proses-proses yang berlaku dalam kilang ini adalah seperti baris-baris kod yang melakukan sesuatu dalam *function* dan roti tersebut adalah hasil akhir yang akan di-*return*-kan pada akhir *function* tersebut.

  

###  **input** 

Dalam Python menyediakan satu fungsi yang dinamakan input(). Input mengambil maklumat daripada *user* untuk disimpan dalam *variable* tertentu.

Kod boleh ditulis seperti berikut;

```python
>>> x = input ('Insert your number here:')
Insert your number here:
```
Untuk menggunakan **input()**, anda perlu meletakkan *prompt*; sebuah arahan untuk diberikan kepada pengguna supaya memasukkan maklumat yang sepatutnya ke dalam program. Di dalam kod di atas, *prompt* yang digunakan adalah 'Insert your number here:'.

*Output prompt* seperti di atas akan terhasil dimana program akan meminta *input* apa ,yang kita mahukan. Selepas menulis apa *input,*  tekan *Enter*. Dan kod akan berjalan seperti biasa.

Penggunaan input() akan menghasilkan kod yang interaktif.

  

##  Loop

Dalam pengaturcaraan, *loop* (*loop*) adalah sebuah konsep dimana beberapa siri perbuatan yang sama yang dilakukan berulang kali.

Sebagai contoh proses untuk memasak sebiji burger.

1. Mulakan dengan mengambil 2 keping roti.

2. Panaskan minyak atas pan.

3. Ambil sekeping daging dan masak.

4. Usai masak, letak daging atas roti tadi.

5. Potong beberapa hirisan timun dan letakkan atas daging.

6. Picit sos dan mayonis keatas timun.

7. Tutup sayur tadi dengan sekeping roti.

8. Siap.

Diatas ini adalah satu proses penuh untuk mencipta seketul burger. Untuk mencipta burger yang seterusnya, maka kita harus melalui proses yang sama.  Seandainya terdapat 100 burger yang anda ingin jual, maka anda akan buat 100 kali *loop* untuk menyiapkan kesemua 100 burger tersebut.

Kerja yang sama dan berulang ini dipanggil sebagai *iteration* *(*iteration). Disebabkan proses manual memasak diatas sangat membosankan kerana berulang,  pengaturcara yang bijak hanya perlu mencipta sebuah *loop* untuk menyiapkan kesemua 100 burger tersebut.

Kod yang mengandungi arahan untuk menjalankan kerja yang sama yang berulang tersebut dipanggil sebagai *loop*.

Selain daripada itu, anda juga boleh meletakkan *conditionl statement* kepada Python seperti, apabila kesemua 100 burger telah siap, sila berhenti (*break*).

Di dalam Python, terdapat dua jenis *loop* iaitu: 

· for *loop*

· while *loop*

Kedua-duanya mempunyai objektif yang sama iaitu untuk mengautomatikkan beberapa siri perbuatan, tetapi terdapat sedikit perbezaan.

###  **For** **loop**

*For loop digunakan untuk menjalankan *iteration* pada struktur data yang *iterable* iaitu *list, tuple,* dan *dictionary*. Untuk menggunakan *for* *loop*, kod seperti berikut akan ditulis iaitu,
```python
for data in y:
	# do*something*1
	# do*something*2
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

Apa yang berada dibawah *for* haruslah diperenggankan (*indent*) bagi menunjukkan arahan tersebut berada dibawah lingkungan *loop* yang dicipta. data mewakili nilai-nilai yang terkandung di dalam list bernama y.

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
*loop* membaca senarai nombor yang berada dalam *list* y dan jika terdapat nilai yang kurang daripada 4, maka hanya nilai tersebut yang akan dikeluarkan *output*. Jika nilai lebih daripada 4, ini memberhentikan proses *loop*.

Selain daripada itu, terdapat satu lagi cara bagi memberhentikan proses *loop* iaitu menggukan **break**.

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
*loop* akan membaca senarai nilai dalam *list*-y. Jika *iteration* menemui nilai yang lebih daripada 4 (iaitu 5 dalam senarai ini), maka *loop* akan berhenti. Tetapi 5 tetap dihasilkan kerana nilai 5 adalah kayu penanda di dalam kod supaya ia diberhentikan. Dalam kod ini, *iteration* setelah menjumpai 5, maka dengan itu, *loop* harus diberhentikan.

Tidak hanya memberhentikan, kita juga boleh menyambung proses *loop* dengan menggunakan kata kunci **continue**.

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
Apabila *iteration* menemui nilai 3, maka *loop* diberitahu supaya meneruskan proses *iteration* hingga ke data terakhir iaitu 5. Nombor 3 tidak terhasil kerana 3 adalah kayu ukur penanda supaya meneruskan *iteration*. Cara ini sangat berguna jika kita ingin memeriksa kewujudan nombor atau string di dalam sebuah list itu. Jika ia wujud, maka teruskan. Jika tidak wujud, iteration tidak akan diteruskan.

Contoh *loop* **for** yang menggunakan **dictionary**:
```python
>>> data = {'nama': 'Jack', 'hobi' : 'badminton'}
>>> for k,v in data.items():
>>> 	print(k,v)
nama Ammar
hobi badminton
```
Kod di atas menggunakan data dalam bentuk **dictionary**. Dalam *loop* for, kod ini telah menggunakan dua *variable* bagi menyimpan elemen-elemen di dalam dictionary iaitu **k** dan **v**.

Data pula telah menggunakan **.items()** dimana salah satu metod Dictionary yang mana berfungsi untuk memasangkan key dan value di dalam dictionary. Apa yang ingin disampaikan adalah, anda boleh menggunakan lebih daripada 1 *variable* di dalam *loop* for bagi menjalankan iteration.

####  **range ( )**

Selain daripad menggunakan list untuk menyenaraikan data, **range()** juga boleh digunakan di dalam *for loop*. **range()** berfungsi bagi menyenaraikan **nombor** dengan julat tertentu.

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

Terdapat sebuah fungsi di yang dapat membantu kod mengira jumlah *iteration* yang telah dilakukan oleh sesebuah *loop*. Fungsi tersebut adalah **enumerate()**.

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

Seperti yang anda dapat lihat pada *output* data di atas, pada setiap elemen di dalam *list* **name**, terdapat nilai indeks yang bersebelahan dengannya yang mengira bilangan *iteration* yang telah dilakukan.

###  **While** **loop**

*While loop* adalah sebuah *loop* yang bertindak menjalankan kod secara berterusan dan berulang selagi mana kod itu menepati syarat yang telah ditetapkan.

*While loop*  yang biasa terdiri daripada 3 komponen asas iaitu:

1. Nilai permulaan

2. Syarat

3. *Increment value*

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

Nilai k adalah **nilai permulaan** supaya *loop* dapat dijalankan. Setelah itu, *loop* diteruskan dengan **syarat**, iaitu selagi mana nilai k  kurang daripada 5, maka *loop* akan diteruskan. Pada *output* pertama iaitu 1, nilai k yang baharu ini akan masuk ke dalam persamaan k += 1  yang sama erti dengan k = k + 1.

Nilai 1 akan masuk pada nilai k. Maka, nilai k yang baru terhasil iaitu k bersamaan dengan 2. Nilai 2 adalah kurang daripada 5, maka *loop* akan berjalan lagi. Proses ini berulang sampailah nilai k sama dengan 5, maka proses lingakaran akan berhenti serta merta.

Seperti juga *for loop*, dalam *while loop* juga menggunakan *break* dan *continue* dengan tujuan yang sama iaitu memutuskan *loop* dan menyambung *loop*. Contoh,

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
Apabila *loop* bertemu dengan nilai k baharu yang bernilai 4, maka *loop* akan terus diberhentikan serta merta.


*Loop* akan melangkau nilai 4 apabila *loop* sampai ke nilai k baharu 4 dan meneruskan *loop* hingga ke nilai 7 dan berhenti.

###  **While** **True**

Dalam *loop*  yang sebelum ini, kita dapat lihat dimana *loop* tersebut mempunyai had tertentu sebelum ia berhenti pada suatu keadaan yang telah ditetapkan.

Namun, kita sebenarnya boleh mencipta *loop* yang berterusan selama-lamanya tanpa ada keadaan yang dapat memberhentikannya.

Dalam Python, kita akan gunakan **while True** untuk mencipta *loop* ini.  

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

Walaubagaimanapun, anda masih lagi boleh meletakkan keadaan untuk memberhentikan *loop* ini seperti yang telah kita pelajari sebelum ini dengan menggunakan katakunci **break****.**

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
*Loop* diatas berhenti apabila mencapai nilai 5.

###  **Carta Alir** 

Di dalam memahami gerak kerja sebuah kod, terdapat satu cara yang dipanggil Carta Alir (*flow chart*). Carta Alir adalah sebuah penerangan visual menggunakan bentuk dan anak panah bagi menerangkan apa yang berlaku dalam sesebuah kod. Secara amnya, bentuk dan kegunaan bentuk itu dapat difahami seperti berikut.

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

Melalui Carta Alir di atas, kita dapat melihat apa yang sedang berlaku di dalam kod yang sedang ditulis. Dimana terdapat pernyataaan *if* dan *elif* yang telah menyebabkan aliran terpecah kepada dua yang memberi syarat kepada input yang diberikan sebelum menuju kepada arahan seterusnya.

Pada laluan x == 5, alirannya adalah **True** maka arahan akan diteruskan melalui aliran ini, manakala pada laluan x > 5, alirannya adalah **False**, maka laluan ini tidak akan digunakan oleh Python.

Carta Alir sangat berguna bagi membayangkan situasi kod lebih lebih lagi jika kod tersebut lebih rumit seperti memunyai pernyataan *if* di dalam pernyataan *if*, mempunyai fungsi di dalam fungsi, mempunyai pernyataan *if* di dalam *loop* dan sebagainya.

Jika anda buntu semasa menulis kod, berundur selangkah ke belakang dan lukis Carta Alir bagi menyusun semula struktur idea dalam minda.

Praktis ini sangat baik dan lama kelamaan, kita dapat membina sendiri Carta Alir di dalam minda sekalipun tanpa melukis di atas kertas.

###  **Nested** **loop** 

*Nested* *loop*  adalah sebuah kod *loop* yang berada di dalam sebuah *loop* yang lain. Perkataan *nested* (sarang) digunakan kerana ia seperti seekor burung yang sedang duduk di dalam sebuah sarang yang mengelilinginya. Struktur *l**oop* ini boleh wujud samada *loop* luarnya adalah *loop*-for di dalamnya *loop*-while, ataupun sebaliknya, ataupun kedua-duanya adalah lingakaran yang sama.

*Nested loop* biasanya digunakan dalam struktur data berbilang dimensi.

-- gambar

Dalam *nested loop*, terdapat 2 jenis *loop* iaitu *loop* luar dan *loop* dalam. *L**oop* luar akan dilaksanakan terlebih dahulu, tetapi sembelum *loop* luar berjaya dilaksanakan dengan sempurna, *loop* dalam akan dilaksanakan barulah *loop* luar akan sempurna.

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
Apa yang terjadi dalam *loop* ini? Mari kita pergi satu persatu.

· Pada baris 3, anda telah menetapkan *variable* yang menyimpan nilai 0, 1, 2 yang dibentuk menggunakan fungsi **range().**

· Kemudian kod mencipta sebuah *loop* tersarang yang terdiri daripada *loop* luar dan *loop* dalam.

· *L**oop* luar akan mengalami *iteration* terlebih dahulu dimana 0, 1, dan 2 akan dihasilkan. Sintaks "*loop* berlangsung..." akan dihasilkan. Tetapi *iteration* ini tidak sempurna selagi mana *loop* dalam tidak menyempurnakan *loop**-*nya terlebih dahulu.

· Anda dapat lihat terdapat pasangan nombor yang terhasil, dimana nombor kiri adalah hasil *loop* luar (*variable-i)*, nombor kanan adalah hasil *loop* dalam (*variable-j)*.

· Maka, pada setiap kali *loop* luar dijalankan, *loop* dalam akan mengambil nilai tersebut dan menjalankan proses *loop* pula padanya. Buktinya dapat dilihat pada *output* apabila nilai 0 terhasil sebanyak tiga kali bersama pasangan nombor 0, 1, dan 2.

· Selepas itu, barulah sintaks "*loop* sempurna" yang membawa maksud *loop* untuk nilai pertama untuk *loop* luar sudah sempurna.

· Kemudian nilai yang seterusnya iaitu 1 pula berlangsung dengan proses  yang sama.

Dibawah penulis sertakan gambaran carta alir bagaimana kod diatas berfungsi; (abaikan time.sleep() kerana ia cuma bertujuan untuk melambatkan proses sintaks bagi memperlihatkan proses *loop*. Anda boleh cuba kod ini pada IDE anda dan lihat hasilnya).

-- gambar

##  Perenggan

· Indentation

Anda dapat perhatikan bahawa apabila bermulanya masuk tajuk *Function* dan *Condition*, terdapat satu cara penulisan yang bermula dengan perenggan atau dikenali sebagai *indentation**.*

Terdapat dua keadaan dimana *indentation* digunapakai iaitu semasa menggunakan *Function* def dan semasa membuat condition. Contoh indentation dalam *Function*,
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
*Nest* juga ada berlaku di dalam for loop dan while loop,
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
*Indentation* sangat penting dalam pembinaan sebuah kod. Ini kerana ia menetukan arahan tersebut di bawah blok yang spesifik.

Dapat diperhatikan di dalam kod while loop, persamaan i = i + 1 berada di luar kod if dimana ini bermaksud persamaan tersebut tertakluk pada while loop. Untuk penjelasan lebih lanjut di dalam gambar dibawah,

-- gambar

Mengikut gambarajah di atas, kod bermula dengan while **True**, dimana ini memberi arahan kepada Python untuk terus menerus menjalankan kod dan menghasilkan *string* “Counting is processed” pada berikutnya. Kod digerakkan menggunakan persamaan **i = i + 1** dan diberikan sebuah kondisi iaitu jika i bersamaan dengan 5, makan kod akan diberhentikan dengan arahan break. Maka terhasillah *output* yang ditunjukkan di atas.

##  **Library**

Secara amnya, *library* adalah satu himpunan kod yang dikumpulkan di dalam satu ruang bernama *package**.* Setiap *library* mempunyai kegunaan tertentu seperti perkiraan Matermaik, membuat graf, mengumpul data dan sebagainya. *Package* pula terdiri daripada himpunan *module* iaitu kod-kod yang menjalankan fungsi tertentu.

Berikut adalah contoh *library* yang seringkali digunakan untuk perkiraan Matematik dan memanipulasi data. Antaranya;

· math

· numPy

· Pandas

· Seaborn

· Matplotlib

Selain daripada itu, terdapat juga *library* yang digunakan untuk proces *web scrapping* iaitu proses mengeluarkan maklumat daripada laman web. *Library* yang digunakan ialah:

· Selenium

· Beautifulsoup

###  **numPy**

Numpy atau Number Python adalah sebuah *library* yang menyediakan fungsi berkaitan dengan matematik dan juga matriks.

Dengan menggunakan numPy, anda boleh mencipta sebuah matriks (*array*) dan melakukan operasi kepadanya.  Mari kita lihat contoh penggunaan numPy.

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
Dalam kod di atas, *array* telah dicipta dengan kod np.array dan ditulis di dalamnya matriks dalam bentuk list. Jika dapat dilihat, ini adalaha matriks 3 X 3, dengan 3 lajur dan 3 baris.

Seterusnya, operasi penolakan dilakukan dan anda dapat lihat ouput kepada kod ini adalah hasil tolak *array* A dan *array* B.

Anda juga boleh menyeru nombor, lajur dan baris di dalam *array* dengan menggunakan index koordinat nombor tersebut.

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

Bagi setiap *library*, terdapat pelbagai modul dan fungsi yang telah tersedia untuk digunakan oleh pengaturcara. Modul dan fungsi ini boleh disemak dengan menggunakan fungsi **dir ()** dengan seperti contoh berikut,

```python
>>> import datetime as dt
>>> dir (dt)
['MAXYEAR','MINYEAR','**builtins**','**cached**','**doc**','**file**','**loader**','**name**','**package**','**spec**','date','datetime','datetime*CAPI','sys','time','timedelta','timezone','tzinfo']
```
# **Ralat**

## **Pengenalan**

Ralat atau *error* adalah sebuah kesalahan yang berlaku semasa dalam penulisan kod yang berpunca daripada pelbagai faktor. Antaranya adalah seperti salah ejaan, tiada perenggan, salah penggunaan metod, kesalahan argumen, jenis data, dan lain-lain lagi.

##  **Nyahpepijat**

Untuk pemula, menulis kod adakalanya menjadi sukar apabila berhadapan dengan ralat. Oleh hal yang demikian, tugas pengaturcara bukan sahaja menulis kod tetapi juga melakukan penyiasatan bagi memeriksa bahagian manakah yang menjadi punca kepada sintaks yang menuju kepada ralat.  Ini yang dipanggil sebagai; nyahpepijat atau *debugging*.

-- gambar 

*Rajah* *7**: Rama-rama di dalam komputer.*

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
Selain daripada ia mengeluarkan mesej yang anda mahukan, ia juga mengeluarkan mesej ralat daripada Python *interpreter* yang menjalankan kod.

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