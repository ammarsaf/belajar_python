#  **Asas Python**

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