# Dataset Final Project Data Analysis

Data ini yang saya gunakan untuk melakukan analisis data dengan menggunakan SQL, Python, dan juga Visualisasi data menggunakan Google Data Studio/Looker Studio pada Final Project Bootcamp Data Analysis di <a href='https://myskill.id'>MySkill.id</a>. Data yang digunakan adalah data yang berasal dari Kaggle: <a href='https://www.kaggle.com/datasets/zusmani/pakistans-largest-ecommerce-dataset'>Pakistan's Largest E-Commerce Dataset</a> dengan beberapa perubahan. Harga yang tertera sudah dikonversi 1 Rupee sama dengan Rp 58.

Dataset yang akan digunakan adalah order_detail, sku_detail, customer_detail, dan payment_detail.
<br>Mengenai penjelasan dataset adalah sebagai berikut:

**order_detail**:
* id 			→ angka unik dari order / id_order
* customer_id 		→ angka unik dari pelanggan 
* order_date 		→ tanggal saat dilakukan transaksi
* sku_id 			→ angka unik dari produk (sku adalah stock keeping unit)
* price			→ harga yang tertera pada tagging harga
* qty_ordered 		→ jumlah barang yang dibeli oleh pelanggan
* before_discount	→ nilai harga total dari produk (price * qty_ordered)
* discount_amount	→ nilai diskon product total
* after_discount		→ nilai harga total produk ketika sudah dikurangi dengan diskon
* is_gross 		→ menunjukkan pelanggan belum membayar pesanan
* is_valid		→ menunjukkan pelanggan sudah melakukan pembayaran
* is_net			→ menunjukkan transaksi sudah selesai 
* payment_id 		→ angka unik dari metode pembayaran

**sku_detail**:
* id 			→ angka unik dari produk (dapat digunakan untuk key saat join)
* sku_name 		→ nama dari produk
* base_price		→ harga barang yang tertera pada tagging harga / price
* cogs 			→ cost of goods sold / total biaya untuk menjual 1 produk
* category		→ kategori produk

**customer_detail**:
* id 			→ angka unik dari pelanggan 
* registered_date	→ tanggal pelanggan mulai mendaftarkan diri sebagai anggota

**payment_detail**:
* id			→ angka unik dari metode pembayaran
* payment_method	→ metode pembayaran yang digunakan
