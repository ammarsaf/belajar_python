===============
OOP
===============

Pengaturcaraan Berorientasi Objek (PBO) atau dalam Inggerisnya, _Object Oriented Programming_ (OOP) adalah sebuah gaya pengaturcaraan yang berkonsepkan _class_ dan _object._

## **_Class_**

_Class_ adalah satu himpunan kod yang terdiri daripada beberapa komponen seperti metod, atribut dan _object_. Terdapat beberapa tujuan pengaturcara menggunakan pendekatan _Class_ iaitu;

1. Untuk menghimpunkan fungsi-fungsi yang mempunyai tujuan umum yang sama diantara satu sama lain.

2. Untuk mencipta modul yang boleh diulang-pakai.

3. Untuk menghimpunkan kod dalam dengan keupayaan keselamatan ke atas kod.

4. Untuk memudahkan proses membangunkan sesebuah sistem/algoritma.

_Nota Ulangkaji_:

Sebelum ini kita telah mempelajari bagaimana caranya kita boleh mencipta _function_ yang dapat menjalankan beberapa baris kod dengan hanya menggunakan nama _function tersebut_.

Bayangkan anda telah mencipta beberapa _function_ yang mempunyai tujuan umum yang sama, misalnya; formula matematik (tambah, tolak, bahagi, darab, kuasa); adalah praktis yang baik untuk menghimpunkan kesemua ini ke dalam satu _class_ supaya mudah untuk digunakan jika diperlukan.

Mari pelajari bagaimana untuk menulis _class:_

1. **_Clas_****_s_**

Pada setiap metod _Class_, perkataan **_class_** akan ditulis di awal kod diikuti dengan nama _Class_ tersebut.

Contoh: Anda ingin mencipta satu _class_ berkenaan himpunan operasi dalam Matematik. Untuk mencipta _class_, tulis kod seperti berikut;

```python
class MathOperation:
```
Anda boleh menggunakan apa apa nama sahaja untuk mencipta _class_ anda yang tersendiri. Penulis menggunakan nama MathOperation untuk _class_ ini.

2. **_Attribute_**

Dalam _class_, a_ttribute_ (atau juga dikenala sebagai _class attribute_) bertindak seperti _variable_ jika di luar _class._ Maklumat ini boleh digunapakai dalam _method_ pada langkah seterusnya.

Di bawah terdapat 2 atribute yang menyimpan maklumat mengenai _class_ dan tarikhnya. Terpulang kepada anda ingin meletakkan maklumat apa pada _atribute_ ini.

```python
>>> class MathOperation:
	info = “This is a simple mathematical operation.”
	date = “4 December 2022”
```
Dalam kod diatas, **info** dan **date** dikenali sebagai _class attribute_.

_Class attribute_ adalah lebih kurang seperti _global_ _variable_. Ia boleh diakses dalam _method_ yang lain dalam _class._

3. **_M_****_ethod_**

Metod atau _call function_ adalah _function_ yang ditulis yang ditulis dalam sebuah _class_. Dalam _class_, di dalam argumen **def** perlu disusuli dengan atribut **self** . Self bertindak sebagai objek kepada _class_ bagi membenarkan metod tersebut untuk mengakses mana mana maklumat yang tertakluk dalam _class_.

```python
class MathOperation:
	info = "This is a simple mathematical operation."
	date = "4 December 2022"
	def get_class_info(self):
		print(“Here is the class info:”, info, date)
```
4. **_Object_**

Untuk melaksanakan _method_ dalam _class,_ anda perlu menulis satu baris yang dipanggil sebagai _object_.

_Object_ digunakan sebagai akses untuk menjalankan _method_ dalam sesebuah _class._ Cara menulis _object_ adalah seperti berikut.

```python
>>> class MathOperation:
	info = 'This is a simple mathematical operation.'
	date = '4 December 2022'
	def get_class_info(self):
		print(“Here is the class info:”, info, date)

>>> my_math = MathOperation()
>>> my_math.get_class_info()

Here is the class info: This is a simple mathematical operation. 4 December 2022
```
**my_math** adalah _object_ dalam _class_ ini. (tindakan ini dikenali sebagai _instantiate an object from the Class)_ Kemudian _object_ ini digunakan untuk mengakses _method_ dalam _class_ iaitu **get_class_info()**yang menghasilkan output info seperti anda dapat lihat diatas.

Mari kita kembangkan lagi kod ini dengan beberapa _method_.
```python
>>> class MathOperation:
		info = 'This is a simple mathematical operation.
		date = '4 December 2022'
	
		val_a = 5
		val_b = 3
	
		def get_class_info(self):
			print(“Here is the class info:”, info, date)
		
		def add_this(self):
			return f'Answer: {val_a + val_b}'
		
		def minus_this(self):
			if val_a > val_b:
				return f'Answer: {val_a - val_b}'
			elif val_b > val_a:
				return f'Answer: {val_b - val_a}'

>>> my_math = MathOperation()
>>> my_math.add_this()

Answer: 2
```
Namun, terdapat **kelemahan** dalam _class_ ini:

1. Untuk anda menjalankan operasi **add_this()**bagi nilai lain, anda tidak punya keupayaan untuk menggunakan nilai lain untuk attribute val_a dan val_b. Ini menjadikan ia leceh kerana anda tidak boleh menggunakan kod ini secara berulang kali; yang mana melanggar tujuan asal sesebuah _class_.

2. Jika _class_ ini dikembangkan lagi dengan beberapa metod, sukar untuk kita generalisasikan nilai bagi operasi tersebut.

Maka, untuk menyelesaikan kelemahan ini, kita akan berkenalan dengan konsep yang baru iaitu _constructor_.

## **_Constructor_** 

Maka, terdapat satu penyelesaian bagi menyelesaikan masalah ini iaitu dengan menggunakan c_onstructor_. Dengan menggunakan c_onstructor,_ nilai **val_a** dan **val_b** tadi tidak perlu ditukar secara terus melalui dalam kod, namun cuma perlu diubah dalam bentuk argumen.

Kita akan lihat dalam kod dibawah;

```python
>>> class MathOperation:
	info = 'This is a simple mathematical operation.'
	date = '4 December 2022'
	def __init__(self, val_a, val_b):
		self.val_a = val_a
		self.val_b = val_b
		self.battery = 10
	def get_class_info(self):
		print('Here is the class info:', info, date)
	
	def add_this(self):
		self.battery -= 1
		return f'Answer: {self.val_a + self.val_b}, op left: {self.battery }'
	
	def minus_this(self):
		self.battery -= 1
		if self.val_a > self.val_b:
			return f'Answer: {self.val_a - self.val_b} battery left: {self.battery }'
	
		elif val_b > val_a:
			return f'Answer: {self.val_b - self.val_a} battery left: {self.battery }'
```
Dalam kod diatas, **val_a** dan **val_b** tadi yang ditulis sebagai atribute telah dipadam dan digantikan dengan satu fungsi yang bernama **__init__()**.

Dengan menggunakan **__init__()**, **val_a** dan **val_b** tadi boleh diakses dalam _object_ itu secara terus dan menyebabkan nilai tersebut boleh diubah hanya dengan menggunakan _object_ tersebut tanpa perlu menukarnya dalam _class_.

17 dan 4 ditulis dalam fungsi **add_this()** dan bukan pada _class attribute_ lagi.

Untuk setiap operasi pula, bilangan bateri akan ditolak daripada bilangan operasi awal sehingga bateri tinggal 0 dan kalkulator tidak boleh digunakan lagi.

_Attribute_ ini dikenali sebagai **_object attribute_**.

**Object attribute**

- Object attribute adalah sebuah attribute yang akan dicipta apabila kita _instantiate_ _the object of the class._

- Dengan menggunakan object attribute, object tersebut mempunyai _state_ yang yang tersendiri yang akan kekal dan berubah.

```python
>>> my_math = MathOperation(17, 4)

>>> print( my_math.add_this())
>>> print( my_math.minus_this())
>>> print( my_math.minus_this())
>>> print( my_math.add_this())

Answer: 13 battery left: 9
Answer: 6 battery left: 8
Answer: 6 battery left: 7
Answer: 13 battery left: 6
```

Dalam output diatas, dapat dilihat nilai _battery left_ berkurangan untuk setiap operasi. Ini bermakna, untuk object my_math, terdapat satu bateri _state_ yang mengekalkan maklumat dan mengubah nilai tersebut apabila berlaku operasi penambahan dan penolakan. Daripada sini kita dapat lihat, dengan menggunakan _object attribute_, kita boleh menggubah sebuah kod yang mempunyai _state_ tersendiri.

### **Perwarisan**

Perwarisan boleh digambarkan seperti perwarisan biologi dalam kehidupan manusia. Seorang anak akan mewarisi ciri-ciri yang terpapar pada ibubapa mereka sama ada tinggi, rendah, cerah, gelap, bermata bundar, bermata sepert dan sebagainya.

 Misalnya anda ingin menulis _class_ yang baru, yang mempunyai kebolehan yang sama dengan _class_ yang sedia ada tetapi dengan sedikit penambahan. Adalah tidak praktikal untuk anda menulis semula _class_ yang sama seperti yang sebelumnya untuk mewujudkan _class_ ini. Maka, cara yang praktikal adalah dengan ‘mewariskan’ apa yang telah ditulis pada _class_ sebelum itu pada _class_  yang baru dan menambah fungsi baharu padanya adalah lebih mudah.

Dalam Python OOP, ini dikenali sebagai _inheritance._

Contoh mudah perwarisan:

```python
>>> class TheParents:	
		def __init__(self, name):
			self.name = name
>>> class TheChild(TheParents):
	pass
```
Dalam kod diatas, _class_ **TheC****hild** telah mewarisi kod daripada _class_ **The****Parent.** Selain daripada mewarisi _method_ daripada Parent, Child juga boleh membentuk _method_ barunya sendiri.

Mari kita kembangkan kod diatas supaya **TheC****hild** sdapat mengembakan _class_ nya daripada **The****Parent****s****.**

```python
>>>> class TheParents:
	     def __init__(self, father_name, mother_name):
	         self.father_name = father_name
	         self.mother_name = mother_name
	     def get_full_info(self):
	         print(self.father_name, self.mother_name)

>>> class TheChild(TheParents):
	     def __init__(self, child_name):
	         self.child_name = child_name
	     def get_all_family(self):
	         super().__init__('Zuhal', 'Nur')
	         self.get_full_info()
	         print(self.child_name)
         
>>> child = TheChild('Mat')

>>> child.get_all_family()

Zuhal Nur
Mat
```
Dalam _class_ TheChild, anda akan lihat terdapat satu _build-in_ function yang baru yang digunakan iaitu **super()**.

**super()** digunakan untuk mewarisi _parent class_ supaya apa yang berada dalam _class_ tersebut akan berada dalam _child class_

