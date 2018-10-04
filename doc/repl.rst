Menggunakan REPL (Read-Evaluate-Print Loop)
=========================================

REPL mengizinkan anda untuk berinteraksi dengan game Pygame Zero yang sedang berjalan menggunakan perintah 
Python. Ketika anda menuliskannya, sistem akan menawarkan sugesti berdasarkan variabel yang ada
pada program anda. Ini bisa berguna untuk melakukan debuggin pada game anda atau menyetel bagaimana tingkat kesulitannya.

.. image:: _static/repl.png

REPL adalah kependekan dari Read-Evaluate-Print Loop; yang berarti:

1. **Read** membaca baris kode yang anda tuliskan
2. **Evaluate** evaluasi kode
3. **Print** menampilkan hasil
4. **Loop** mengulang kembali ke tahap 1!

Ini adalah *fitur pilihan* yang mungkin perlu :ref: `di install
<install-repl>` jika awalnya tidak terinstall dengan Pygame Zero. jika anda mencoba
menggunakan REPL, Pygame Zero akan memberitahu anda jika itu sudah terinstall atau belum.


Menjalankan program Pygame Zero dengan REPL
-------------------------------------------

Jika normalnya anda menjalankan program Pygame Zero anda menggunakan terminal, tambahkan ``--repl``
pada command line ketika menjalankan ``pgzrun``. Contohnya, jika game anda ada pada
sebuah file bernama ``mygame.py``, jalankan::

    pgzrun --repl mygame.py


Menggunakan REPL
----------------

Kode Python yang sudah anda tulis pada REPL dievaluasi seolah-olah anda menuliskannya
pada file game anda.

Contohnya, jika game anda menggandung kode ::

    alien = Actor('alien', pos=(54, 60))

    def draw():
        screen.clear()
        alien.draw()


Maka pada REPL anda bisa menuliskan ``alien`` untuk melihat objek alien::

    >>> alien
    <Actor 'alien' pos=(54, 60)>

Anda bisa menentukan atribut pada objek ``alien`` dan melihatnya bergerak::

    >>> alien.x = 90
