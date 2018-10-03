Menjalankan Pygame Zero di IDLE dan IDE lainnya
==========================================

.. versionadded:: 1.2

Pygame Zero biasanya dijalankan dengan menggunakan perintah seperti::

    pgzrun my_program.py

Program tertentu, misalkan lingkungan pengembangan terintegrasi *(integrated development environments)* seperti IDLE dan
Edublocks, hanya akan menjalankan ``python``, bukan ``pgzrun``.

Pygame Zero menyertakan sebuah jalan untuk menuliskan program Python yang dapat dijalankan menggunakan ``python``. Untuk melakukannya, taruh ::

    import pgzrun

sebagai baris paling awal dari program Pygame Zero dan taruh ::

    pgzrun.go()

sebagai baris paling akhir.


Example
-------

Ini merupakan program Pygame Zero yang menggambar sebuah lingkaran. Anda dapat menjalankan program ini dengan menyalin kode ini ke IDLE::


    import pgzrun


    WIDTH = 800
    HEIGHT = 600

    def draw():
        screen.clear()
        screen.draw.circle((400, 300), 30, 'white')


    pgzrun.go()

