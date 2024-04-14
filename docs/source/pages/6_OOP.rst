===============
OOP
===============

Pengaturcaraan Berorientasi Objek (PBO) atau dalam Inggerisnya, *Object Oriented Programming* (OOP) adalah sebuah gaya pengaturcaraan yan  berko sepkan *class* *object.

--------------------
**Class**
--------------------

*Class* adalah satu himpunan kod yang terdiri daripada beberapa komponen seperti metod, atribut dan objek. Terdapat beberapa tujuan pengaturcara menggunakan pendekatan *Class* iaitu;

1. Untuk menghimpunkan fungsi-fungsi yang mempunyai tujuan umum yang sama diantara satu sama lain.

2. Untuk mencipta modul yang boleh diulang-pakai.

3. Untuk menghimpunkan kod dalam dengan keupayaan keselamatan ke atas kod.

4. Untuk memudahkan proses membangunkan sesebuah sistem/algoritma.

*Nota Ulangkaji*:

Sebelum ini kita telah mempelajari bagaimana caranya kita boleh mencipta *function* yang dapat menjalankan beberapa baris kod dengan hanya menggunakan nama *function* tersebut.

Bayangkan anda telah mencipta beberapa *function* yang mempunyai tujuan umum yang sama, misalnya; formula matematik (tambah, tolak, bahagi, darab, kuasa); adalah praktis yang baik untuk menghimpunkan kesemua ini ke dalam satu *class* supaya mudah untuk digunakan jika diperlukan.

Mari pelajari bagaimana untuk menulis _class:_

1. *Class*

Pada setiap metod Class, perkataan *class* akan ditulis di awal kod diikuti dengan nama *Class* tersebut.

Contoh: Anda ingin mencipta satu *class* berkenaan himpunan operasi dalam Matematik. Untuk mencipta *class*, tulis kod seperti berikut;

.. code-block:: python

	class MathOperation:

Anda boleh menggunakan apa apa nama sahaja untuk mencipta *class* anda yang tersendiri. Penulis menggunakan nama MathOperation untuk *class* ini.

2. Attribute 

Dalam *class*, *attribute*  (atau juga dikenala sebagai *class attribute*) bertindak seperti *variable* jika di luar *class*. Maklumat ini boleh digunapakai dalam *method* pada langkah seterusnya.

Di bawah terdapat 2 atribute yang menyimpan maklumat mengenai *class* dan tarikhnya. Terpulang kepada anda ingin meletakkan maklumat apa pada *atribute* ini.

.. code-block:: python

	class MathOperation:
		info = "This is a simple mathematical operation."
		date = "4 December 2022"

Dalam kod diatas, ``info`` dan ``date`` dikenali sebagai *class attribute*.

*Class attribute* adalah lebih kurang seperti *global variable*. Ia boleh diakses dalam *method* yang lain dalam *class*.

3. *Method*

Metod atau _call function_adalah_function_yang ditulis yang ditulis dalam sebuah *class*. Dalam *class*, di dalam argumen ``def`` perlu disusuli dengan atribut ``self`` . Self bertindak sebagai objek kepada *class* bagi membenarkan metod tersebut untuk mengakses mana mana maklumat yang tertakluk dalam *class*.

.. code-block:: python

	class MathOperation:
		info = "This is a simple mathematical operation."
		date = "4 December 2022"
		def get_class_info(self):
			print(“Here is the class info:”, info, date)

4. *Object*

Untuk melaksanakan *method* dalam _class,_ anda perlu menulis satu baris yang dipanggil sebagai *object*.

*Object* digunakan sebagai akses untuk menjalankan *method* dalam sesebuah *class*. Cara menulis *object* adalah seperti berikut.

.. code-block:: python

	class MathOperation:
		info = 'This is a simple mathematical operation.'
		date = '4 December 2022'
		def get_class_info(self):
			print(“Here is the class info:”, info, date)

	my_math = MathOperation()
	my_math.get_class_info()

Here is the class info: This is a simple mathematical operation. 4 December 2022

*my_math* adalah *object* dalam *class* ini. (tindakan ini dikenali sebagai _instantiate an object from the Class)_ Kemudian *object* ini digunakan untuk *mengakses method* dalam *class* iaitu ``get_class_info()`` yang menghasilkan output info seperti anda dapat lihat diatas.

Mari kita kembangkan lagi kod ini dengan beberapa *method*.

.. code-block:: python

	class MathOperation:
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
	my_math = MathOperation()
	my_math.add_this()

	Answer: 2

Namun, terdapat **kelemahan** dalam _class_ ini:

1. Untuk anda menjalankan operasi ``add_this()`` bagi nilai lain, anda tidak punya keupayaan untuk menggunakan nilai lain untuk attribute val_a dan val_b. Ini menjadikan ia leceh kerana anda tidak boleh menggunakan kod ini secara berulang kali; yang mana melanggar tujuan asal sesebuah `class`.

2. Jika ``class`` ini dikembangkan lagi dengan beberapa metod, sukar untuk kita generalisasikan nilai bagi operasi tersebut.

Maka, untuk menyelesaikan kelemahan ini, kita akan berkenalan dengan konsep yang baru iaitu *constructor*.

--------------------
Constructor
--------------------

Maka, terdapat satu penyelesaian bagi menyelesaikan masalah ini iaitu dengan menggunakan *constructor*.Dengan menggunakan *constructor*, nilai ``val_a`` dan ``val_b`` tadi tidak perlu ditukar secara terus melalui dalam kod, namun cuma perlu diubah dalam bentuk argumen.

Kita akan lihat dalam kod dibawah;

.. code-block:: python

    class MathOperation:
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

Dalam kod diatas, ``val_a`` dan ``val_b`` tadi yang ditulis sebagai atribute telah dipadam dan digantikan dengan satu fungsi yang bernama ``__init__()``.

Dengan menggunakan ``__init__()``, ``val_a``dan ``val_b`` tadi boleh diakses dalam ``object`` itu secara terus dan menyebabkan nilai tersebut boleh diubah hanya dengan menggunakan ``object`` tersebut tanpa perlu menukarnya dalam ``class``.

17 dan 4 ditulis dalam fungsi ``add_this()`` dan bukan pada _class *attribute* lagi.

Untuk setiap operasi pula, bilangan bateri akan ditolak daripada bilangan operasi awal sehingga bateri tinggal 0 dan kalkulator tidak boleh digunakan lagi.

*Attribute* ini dikenali sebagai *object attribute*.

------------------------------
Object attribute
------------------------------

- Object attribute adalah sebuah attribute yang akan dicipta apabila kita *instantiate* objek kelas tersebut.

- Dengan menggunakan object attribute, object tersebut mempunyai *state* yang yang tersendiri yang akan kekal dan berubah.

.. code-block:: python
	my_math = MathOperation(17, 4)

	print( my_math.add_this())
	print( my_math.minus_this())
	print( my_math.minus_this())
	print( my_math.add_this())

.. code-block:: python
	Answer: 13 battery left: 9
	Answer: 6 battery left: 8
	Answer: 6 battery left: 7
	Answer: 13 battery left: 6

Dalam output diatas, dapat dilihat nilai *battery left* berkurangan untuk setiap operasi. Ini bermakna, untuk object my_math, terdapat satu bateri *state* yang mengekalkan maklumat dan mengubah nilai tersebut apabila berlaku operasi penambahan dan penolakan. Daripada sini kita dapat lihat, dengan menggunakan *object attribute*, kita boleh menggubah sebuah kod yang mempunyai *state* tersendiri.

---------------------------
Perwarisan
---------------------------

Perwarisan boleh digambarkan seperti perwarisan biologi dalam kehidupan manusia. Seorang anak akan mewarisi ciri-ciri yang terpapar pada ibubapa mereka sama ada tinggi, rendah, cerah, gelap, bermata bundar, bermata sepert dan sebagainya.

Misalnya anda ingin menulis *class* yang baru, yang mempunyai kebolehan yang sama dengan *class* yang sedia ada tetapi dengan sedikit penambahan. Adalah tidak praktikal untuk anda menulis semula *class* yang sama seperti yang sebelumnya untuk mewujudkan *class* ini. Maka, cara yang praktikal adalah dengan 'mewariskan' apa yang telah ditulis pada *class* sebelum itu pada *class*  yang baru dan menambah fungsi baharu padanya adalah lebih mudah.

Dalam Python OOP, ini dikenali sebagai *inheritance*.

Contoh mudah perwarisan:

.. code-block:: python
	class TheParents:	
		def __init__(self, name):
			self.name = name
	class TheChild(TheParents):
	pass

Dalam kod diatas, ``class TheChild`` telah mewarisi kod daripada ``class TheParent``. Selain daripada mewarisi ``method`` daripada Parent, Child juga boleh membentuk *method* barunya sendiri.

Mari kita kembangkan kod diatas supaya **TheC****hild** sdapat mengembakan _class_ nya daripada **The****Parent****s****.**

.. code-block:: python
	class TheParents:
	def __init__(self, father_name, mother_name):
		self.father_name = father_name
		self.mother_name = mother_name
	def get_full_info(self):
		print(self.father_name, self.mother_name)

.. code-block:: python
	class TheChild(TheParents):
		def __init__(self, child_name):
			self.child_name = child_name
		def get_all_family(self):
			super().__init__('Zuhal', 'Nur')
			self.get_full_info()
			print(self.child_name)
	child = TheChild('Mat')
	child.get_all_family()

.. code-block:: python
	Zuhal Nur
	Mat

Dalam ``class TheChild``, anda akan lihat terdapat satu *build-in function* yang baru yang digunakan iaitu ``super()``.

``super()`` digunakan untuk mewarisi _parent class_supaya apa yang berada dalam ``class`` tersebut akan berada dalam *child class*.

