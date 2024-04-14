=============
IDE
=============

Sebelum mempelajari Python dengan lebih lanjut,  perlu diketahui bahawa kod pengaturcaraan mempunyai alat tertentu supaya kita boleh jalankan kod tersebut. Teknologi penulisan berkembang pada zaman dahulu bermula dengan manusia menulis di atas batu, kulit haiwan, dinding gua dan sebagainya. Kemudian muncul inovasi kertas dan manusia mula menulis di atas kertas. Teknologi semakin berkembang dan wujudlah komputer dimana manusia mula menulis menggunakan dalam perisian yang kita kenali seperti Microsoft Words. Selari dengan perkembangan teknologi, medium penulisan kod juga muncul bagi memudahkan gerak kerja pengaturcaraan.

Medium ini dinamakan sebagai *Integrated Development Environment* (IDE). Pada masa kini terdapat pelbagai IDE yang telah dicipta untuk kegunaan pengaturcara.

------------------------------------
Skrip dan Notebook
------------------------------------

Untuk menulis kod Python, anda boleh memilih untuk menulis kod dengan sama ada menggunakan fail berformat skrip (fail .py, sebutan dot pi-wai) ataupun fail berformat *Notebook* (fail ipynb)

Kedua-dua format ini akan menghasilkan output yang sama, tetapi mempunyai sedikit perbezazan kegunaan. Untuk pemula, penulis menyarankan untuk menggunakan Notebook untuk menulis kod.

------------------------------------
Notebook
------------------------------------

Notebook adalah sebuah format fail yang digunakan untuk menulis kod Python. Fail berformat Notebook akan diakhiri dengan **_ipynb_****.**

------------------------------------
Anaconda
------------------------------------

Bagi menulis kod dalam fail berformat ini, penulis menyarankan anda untuk memuat turun Anaconda Navigator. Penulis meletakkan Anaconda sebagai pilihan pertama kerana perisian ini menyediakan pelbagai jenis IDE yang masyhur untuk digunakan bagi menjalankan Python. Anaconda menyediakan IDE seperti Jupyter Notebook, VisualCode, Spyder, dan lain-lain. Penulis meyarankan anda menggunakan *Jupyter Notebook* untuk permulaan.

-- logo anacoda--

Untuk pemasangan perisian Anaconda, ikuti langkah berikut:

1. Muat turun Anconda Navigator daripada [https://docs.anaconda.com/anaconda/install/windows/](https://docs.anaconda.com/anaconda/install/windows/)

2. Klik ikon Anaconda.

3. Anda boleh memilih mana-mana IDE yang berada di dalam Anaconda. IDE yang disarankan adalah *Jupyter Notebook*.

4. Kod Python boleh ditulis dan dijalankan secara terus daripada sini.

------------------------------------
Google Colab
------------------------------------

Untuk menggunakan Google Colab, anda tidak perlu memuat turun apa apa perisian jika ingin menggunakan perkhidmatan ini. Cuma perlu membuat carian “Google Colab” di Google, kemudian anda boleh terus menulis kod di sana.

-- logo Google Colab

Google Colab menggunakan format *Notebook* beserta fungsi-fungsi lain yang sangat berguna terutamanya kepada mereka yang baru bermula dengan pengaturcaraan. Anda hanya perlu mempunyai email Google untuk menggunakan Google Colab tanpa perlu mengikut apa-apa langkah pemasangan perisian.

------------------------------------
Skrip
------------------------------------

Skrip adalah sebuah format fail yang digunakan untuk menulis kod dalam Python. Fail ini akan diakhiri dengan ``.py``  pada nama fail tersebut. Sebagai contoh, project.py.

------------------------------------
Menggunakan CMD
------------------------------------

Untuk menghasilkan output daripada fail skrip, anda perlu menggunakan CMD.

CMD atau **Command Prompt** adalah sebuah antaramuka baris-perintah (command-line interface) yang boleh menjalankan perintah, melakukan fungsi tadbir lanjut dan menyelesaikan beberapa masalah dalam Windows. Kita boleh menulis arahan tertentu di sini untuk diberikan kepada komputer.

Bagi menjalankan kod Python menggunakan CMD, langkah-langkah berikut perlu dijalankan terlebih dahulu.

1. Tulis kod mudah di atas Notepad.

2. Tulis kod berikut (usah risau, anda akan memahami maksud kod ini pada topik seterusnya)

.. code-block:: python
    
    print('Hello world!')

3. Simpan fail dengan ``.py`` pada akhir fail tersebut.

4. Tekan pada bahagian fail yang anda simpan kod Python tersebut.

-- gambar 

5. Tulis CMD pada bahagian *path* dan klik (*enter*).

-- gambar

7. Tulis “python”. (pastikan tiada kesalahan ejaan)

8. Diikuti dengan nama file Python (pastikan di akhir fail Python mempunyai **.py**)

-- gambar

9. Tekan (*enter*).

10. Output `hello world`` akan terpapar dalam CMD.

------------------------------------
Perbandingan IDE
------------------------------------
.. list-table:: Perbezaan Antara IDE

    * - Metod/IDE
      - Kebaikan
      - Kelemahan
    * - Notepad++/Atom/Sublime Text/VSCode  
      - Melakukan projek ataupun aplikasi yang menggunakan lebih daripada 1 fail Python. Aestetik dan cantik. Menyediakan mod pelbagai. 
      - Terdapat sesetengah *module* dan *library* yang perlu diimport dan tidak tersedia dalamnya. |
    * - Spyder (Anaconda) 
      - Sesuai untuk kerja berkaitan dengan Matematik dan Sains kerana telah terbina *library* dan modul yang bersesuaian di dalamnya.
      - Kod tidak boleh dijalankan per blok. Bermaksud untuk menjalankan kod baharu, perlu fail yang baharu.Kurang mesra untuk pemula.
    * - Jupyter Notebook (Anaconda)
      - Sesuai untuk kerja berkaitan dengan Matematik dan Sains kerana telah terbina *library* dan modul yang bersesuaian di dalamnya. Kod boleh dijalankan per blok. *Output* yang terhasil jelas dan baik. Mesra untuk pemula. 
      - Tidak sesuai untuk digunakan jika mahu melakukan projek yang besar yang menggunakan lebih daripada 1 fail Python. Kesukaran untuk mengimport *module* atau *library* sendiri.
    * - Google Colab 
      - Sesuai untuk kerja berkaitan dengan Matematik dan Sains kerana telah terbina *library* dan modul yang bersesuaian di dalamnya. Mesra untuk pemula. Punya mod gelap. 
      - Tidak sesuai untuk digunakan jika mahu melakukan projek yang besar yang menggunakan lebih daripada 1 fail Python. Kesukaran untuk mengimport *module* atau *library* sendiri.

Nota kaki:

Untuk permulaan, penulis menyarankan anda menggunakan **Jupyter Notebook** atau **Google Colab** kerana lebih mudah untuk digunakan.