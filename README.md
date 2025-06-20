# Image-to-ASCII-Converter# 🖼️ 

Skrip Python ini digunakan untuk mengonversi gambar menjadi seni ASCII (ASCII Art) dan menyimpannya ke dalam file `.txt`. Program ini dirancang untuk dijalankan di lingkungan seperti **Google Colab**, karena menggunakan fitur unggah dan unduh dari `google.colab`.

## 📋 Fitur

- Mengunggah gambar langsung dari komputer pengguna
- Mengonversi gambar ke seni ASCII berdasarkan tingkat kecerahan
- Menampilkan hasil ASCII langsung di notebook
- Menyimpan hasil ke dalam file `ascii_art.txt` dan mengunduhnya secara otomatis

## 🛠️ Teknologi yang Digunakan

- Python
- `Pillow (PIL)` untuk manipulasi gambar
- `google.colab.files` untuk upload dan download file
- `IPython.display` untuk menampilkan hasil

## 🚀 Cara Kerja

1. **Unggah Gambar**
   - Pengguna diminta untuk mengunggah gambar melalui antarmuka Google Colab.

2. **Ubah Ukuran & Konversi Grayscale**
   - Gambar diubah ukurannya sesuai `output_width` (default 100) dengan mempertahankan rasio aspek, lalu dikonversi menjadi gambar grayscale.

3. **Pemetaan ke ASCII**
   - Setiap pixel grayscale dikonversi menjadi karakter ASCII dari set ` .:-=+*#%@` sesuai intensitas warnanya.

4. **Bangun ASCII Art**
   - Karakter disusun dalam baris untuk membentuk visual dari gambar.

5. **Output**
   - ASCII Art ditampilkan langsung di notebook.
   - Disimpan ke `ascii_art.txt` dan diunduh secara otomatis.

## 📄 Contoh Output (`ascii_art.txt`)

```text
@@@@@@@@@@@@%@@@@@@@@@@@@@@@@@@@@@@@@@@@@@%%%%%%%%%%######**####*#%######%%#####%%%%%%%%%%%%%%@@@@@@
@@@@@@@@@@@@%@@@@@@@@@@@@@@@@@@@@@@@@@@@%%%%%%%%%%#########*####*###########%%%%%%%%%%%%%%%@@@@@@@@@
@@@@@@@@@@@@%@@@@@@@@@@@@@@@@@@@@@@@@%%%%%%%%%%%%##########**###**#############%%%%%%%%%%%%@@@@@@@@@
@@@@@@@@@@@@%@@@@@@@@@@@@@@@@@@@@@@%%%%%%%%%%%%%##%%##***++++++++****####*########%%%%%%%%%@@@@@@@@@
@@@@@@@@@@@@%@@@@@@@@@@@@@@@@@@@%%%%%%%%%%%%%%%%%#*#**++===++++++++++**#**############%%%%%@@@@@@@@@
@@@@@@@@@@@@%@@@@@@@@@@@@@@@%%%%%%%%%%%%%%%%%%%%%#*+***+++++++++++++++++*#####%#######%%%%@@@@@@@@@@
@@@@@@@@@@@%%@@@@@@@@@@@%%%%%%@@@@@%%%%%%%%%%%%%%*+*#****++++++*++++++*#*+*######%%##%%%%%@@@@@@@@@@
@@@@@@@@@@@%%%@%%%%@@%%%%%%%%@@@@@%%%%%%%%%%%%%#***##***+++++++*++++***+++++*###%%%@@@@%%@@@@@@@@@@@
@@@@@@@@@%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#**##****++++=++++*+++++*++**#**#%@@@@@@@@@@@@@@@@@@@@
@@@@@@@@@%%%%%%%%%%%%%%%%%%%####%%%%%%%%%%%%%#****+*#*++++=++**%%*#%#**%###%%%%%@@@@@@@@@@@@@@@@@@@@
@@@@@@@@%%%%%%%%%%%%%%%%%%@@@@%%%%%%%%%%%%%%%****+*#*+**++#%%%%%#%%%%%#%@@%#@@@@%@@@@@@@@%@@@@@@@@@@
@@@@@@%%%%%##%%%%%%%%%%%@@@@@@@@@%%%%%%%%%%%*******#*#%*+#%@%%%%%%%%%@%%@%%%%@@@@@@%%%@@@@@@@@@@@@@@
@@%%%%%%%#####%%%%%####%@@@@@@@@@%%%%%%%%%%******####%**#%@@%%%#%%%%%@%#%%@@%%@@@%@@@@@%@@@@@@@@@@@@
%%%%%###***###########%%@@@@@@@@%%%%%%%%%%#*****#%##%*##%%@@%%%#@%%@%@@%%@@@@@@@@@%@@@@@@@@@@@@@@@@@
%####***#######***##%%%%%@@@@@%%%%%%%%%%#*+****#%%*##*##%%@@%%#%@#%%%@@%%@@@@@@@@@%%@@@@@@@@@@@@@@@@
#*****#######***##%%%%%%%%%%%%%%%%%%%%*===*#***%%####%@##%%%%%%%%#%%@@@%%@@@@@@@@@%%%@@@@@@@@@@@@@@@
++***####****##%%%%%%%%%%%%%%%%%**#%%+-:-+#***#%%#%#%@@%%%%%%#%%%#%%@@@%@@@@%@@@@@%%%@%%@@@@@@@@@@@@
**********##%%%%%%%%%%%%%%%%%%%%+==+**=--*#***##**=+*#%%%%%%%%@%%#%%%%%%@@%@%@@@%%#*%@@@@@@@@@@@@@@@
********##%%%%%%%%%%%%%%%%%%%%%%+=---=*#*******##*==--=#%@%%%@@%%%%%%%#%@%%@%@@%*#**%#%@@@@@@@@@@@@@
*****##%%%%%%%%%%%%%%%%%%%%%%%%%+------+#%#****%@%%%#*##%%@%%@@@%%%@@%%%%%@@%@@##*=*##%@@%%%%@@@@@@@
**##%%%%%%%%%%%%%%%%%%%%%%%%%%%%*--------=#%*+=%%%%%@@@@%%@@@@@%##%%@%%%%%@%@@@#*+*#%%%@%%%%%%@@@@@@
##%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%*----------+%*+#%%%@@@@@@%%%@@%##*-+#%%%%%@%@@@@###@@%%%%%@@@@@@@@@@
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%##*------------*%%#%@@@@@@@@@@@@@@@%++=+*%%@%@@@@*#@%@@@%@@@@@@@@@@@@@
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%###*-------------=%@%%@@@@@@@@@@@@@@@%%#*+*%%%@@@**#@%@@%%@@@@@@@@@@@@@
%%%%%%%%%%%%%%%%%%%%%%%%%%%#####*--:------------#@%%%%%@@@@@@@%@@@%%@%#%%%@@%**%#@%@@%*%@@@@@@@@@@@@
%%%%%%%%%%%%%%%%%%%%%%%%%#######*=+=------------=###############%%%%%%%#%%%%#*%%*%#@@%**#@@@@@@@@@@@
%%%%%%%%%%%%%%%%%%%%%%%%#########*+*#+----------+**=+*************#########*#*%@*##@@%***#@@@@@@@@@@
%%%%%@@@@@@@@%%%%%%%%%###########*+==#=---------+*+=+***********##############%%*+%@#+****%@@@@@@@@@
#%%@@@@@@@@@@@%%%%##############***%+-=---------**+=*************############*+==###++****#@@@@@@@@@
%%@@@@@@@@@@@@@%%#######%%########++%+----------**+=*************###########*==+*@***+****#%@@@@@@@@
%@@@@@@@@@@@@@@%######%%%###+=+##+#+*+----------**==*************###########*++#%@#+*****#%@@@@@@@@@
@@@@@@@@@@@@@@@%######%%###**+**#=*#*=---------=**==+*************#########*#%%%%@%+****#%@@@@@@@@@@
%@@@@@@@@@@@@@%############*+****+=*=----------=*+==+++++**********########%@@%%%@@###%%@@@@@@@@@@@@
%@@@@@@@@@@@@%####**#####++--+**+++=-----------=++==+++++++********#**####%@@@@%%@@@@@@@@@@@@@@@@@@@
#%%@@@@@@@%#####**#*#####+=---**++=-=----------=+=-===+++++++*****+=*%%%%#@@%%@@@@@@@@@%%%%@@@@@@@@@
##############**##*######=-==--++=-=--=--------=+=-====++++++++++==*#*+*%@@%%%@@@@@@@@@%%%%%@@@@@@@@
#######**####****++######-:=--======----=------=+=-=====+++=====-=+###%##@@%@@@@@@@@@@@%%%%@@@@@@@@@
###*********+++=++*#####*------=====---===-----=+--=============+**##%%%@@@@@@@%###%%@%#%%%%@@@@@@@@
***********++++*++#####+:----:-====-=-=====-:--==--==============*#%%%@@@@@@@%*****%%%%%%##%%%%@@@@@
*********+++***=:+###+-:-=---:-===========-::--==--==============++++*#@@@@@@*+****%%%%%%%%%@@%%@@@@
************++-:-#*=---===---.---=========--=====-=============++++=+++*@@@@@#*####%%%%%###%@@@@@@@@
*********++++-:.=-:--====--+- ---====-==================+======**#*#@%#+%@@@@%*#%%%%%%%%##%%@@@@@@@@
******#*++**+:.::-=---===-=+-.:--=-==-=-=============++++++++*++*#*%@#++%@@@@@%%%%%%%%@@@%%@@@@@@@@@
***++**+***++::-==---====-=*=::-----=--========+++++*****#####*+*##@#+++#@@@@%%%%%#%%@@@@@@@@@@@@@@@
***=*#++*#*+=:====--=-=---=*+-.-----=--======++***############*+#%%#+++*#%%@%%%%%%%%@@@@@@@@@@@@@@@@
***=**=+**++-=====--------=*==::------=====++***#############%**%@#+++*%%%%%%%%%#%%%@@@@@@@@@@@@@@@@
***+******+*+=====--====---++-::------=-==+******#############*#@#+++*%%%%%%%%%%##@%@@@@@@@@@@@@@@@@
***#*****+++============---=+=::---------==*+*****############+%#++++%%%%%%%%%#%%#%@@@@@@@@@@@@@@@@@
+******+==============---=-===::----------===+++**###########+#*+==+%%%%%%#####%@%@@@@@@@@@@@@@@@@@@
:-=++============-=========--:.------------==--===++***#*##*+*+-===%%%%%%%**##%@@@@@@@@@@@@@@@@@@@@@
:::::---==--====---=======--.-:---------------========+++++=++-=+=-%%%%%%*+*#%%@@@@@@@@@@@@@@@@@@@@@
::::::::---------====-----=-=*=:----------------==================-#%%%%#+*##%%%@@%%@@@@@@@@@@@@@@@@
:::::::::::--=--------:..=****+------------------==============+++=+%%%%+*##%%%%@@@@@@@@@@@@@@@@@@@@
::::::::::::::-----:::.:+++****+-:-------------------====-======+++-#%%***#%%%%%@@@@@@@@@@@@@@@@@@@@
::::::::::::::::::::-++**+*******=------------------------======+++-+%#**#%%%#%%@@@@@@@@@@@@@@@@@@@@
:::::::::::::::::::::=++***********=-----------------------=====+++=-***#%%%%##%@@@@@@@@@%@@@@@@@@@@
:::::::::::::::::::::::-=*##*****##**+=------------------:========++==+*#%%%%%%%%%%@@@@@%%@@@@%@@@@@
::::::::::::::::::::::::::-=+***##****#*==----------------============*#%%##%%%#%%@@@@%%%%%%%%%@@%@@
:::::::::::::::::::::::::::::--+##***##**##++===---=====+==========+=+#%%#####%##%@@%%%%%%%%%%%%%%@%
::::::::::::::::::::::::::::::::-=+*##*####***#*+*#*#***+--========++###%#******%%%%##%%%%%%%%%%%%%%
::::::::::::::::::::::::::::::::::::=+####**##***##*###*+---=======++####*+****#%###%#%%%%%%%%%%%#%%
:::::::::::::::::::::::::::::::::::::::=+******####*###*+---=======++###***+**##########%%%%%%%###%%
::::::::::::::::::::::::::::::::::::::::::-+*#####**###*=-=========++*#**#######*****##%%%%%%%###%%#
:::::::::::::::::::::::::::::::::::::::::::::-+****###**=========++++****%%%%##%%%%%%%%%%%%%%%######
::::::::::::::::::::::::::::::::::::::::::::::::-+*#%#+*=========+++++++#%%%%%##%%%%%%%%%%%%########
:::::::::::::::::::::::::::::::::::::::::::::::::::=++*+:-=======+++++++*%%%%%%##%%%#%##############
::::::::::::::::::::::::::::::::::::::::::::::::::::::==::-=======++++++*#%%%%%%##%%##########**####
::::::::::::::::::::::::::::::::::::::::::::::::::::::::-::-========+++++###%%%%%##%%%#********#####
::::::::::::::::::::::::::::::::::::::::::::::::--------------======++++**#%#%%%%###%%%%#**#########
:::::::::::::::::::::::::::::::::::::::---------------------===++++++++****##%%%%%#*#%%%%###########
:::::::::::::::::::::-:-:-::::::::::----------------=====++++++++++++*+****##%%%%%#**#%%%%##%%%%%%%%
:::::::::::::::::----------------------------=====+++++++++++++++++++++*****##%%%%##*#%%%%%%@@@@@@@@
:::::::::::::::-------=---------------======+++++++++++++++++++++++++++++***###%%%####%%%%%%@@@@@@@@
--::::::::-------========------------=+++++++++++++++++++++++++++++++++++++****#%#####%%%%%%%@@@@@@@
-------------============----------==++++++++++++++++++++++++++++++++++++++*****######%%%%%%%@@@@@@@
-=----------==============---=--===+++++++++++++++++++++++++++++++++++++++++*******###%%%%%%%%@@@@@@
===---=======================++++++++++++++++++++++++++++++++++++++++++++++*****+**###%%%%%%%%@@@@@@
===============================+++++++++++++++++++++++++++++++++++++++++++++**+++*#####%%%%%%%%@@@@@

