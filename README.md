# **Travel Insurance**

## **Context**
Perusahaan asuransi travel ingin mengetahui perilaku pelanggan terkait klaim asuransi dengan cara mengidentifikasi pola atau faktor yang mempengaruhi keputusan pelanggan apakah akan mengajukan klaim asuransi atau tidak. Data yang dipakai meliputi agency, agency type, distribution channel, product name, duration, destination, net sales, commision, age, dan sejarah klaim.
Target:
0 : Nasabah tidak mengajukan klaim asuransi
1 : Nasabah mengajukan klaim asuransi

## **Problem Statement**
Perusahaan asuransi travel menangggung biaya yang akan diklaim oleh nasabah berdasarkan tipe produk asuransi yang dipilih oleh nasabah. Biaya yang diklaim meliputi kerugian nasabah selama perjalanan. Untuk menghindari kerugian yang besar, perusahaan ingin melakukan prediksi terhadap nasabah yang  berpotensi mengajukan klaim dan yang tidak agar sesuai dengan produk serta premi yang dibayarkan.

## **Goals**
Perusahaan dapat membangun model prediksi yang dapat mengklasifikasikan nasabah yang berpotensi mengajukan klaim asuransi dan nasabah yang kemungkinan besar tidak akan mengajukan klaim. Prediksi ini dilakukan untuk menghindari kerugian akibat nasabah yang mengajukan klaim tetapi melebihi premi yang sudah dibayarkan.

## **Analytic Approach**
Menganalisis data untuk menemukan pola atau faktor yang mempengaruhi nasabah mengajukan klaim asuransi travel atau tidak.
Kemudian membangun model kalsifikasi yang membandtu perusahaan untuk memprediksi probabilitas nasabah yang akan mengajukan klaim asurasni atau tidak.

## **Metric Evaluation**
Type 1 error: False Positive
<br>
Konsekuensi: Perusahaan mengalami kerugian karena nasabah tidak mengajukan klaim

Type 2 error: False Negative
<br>
Konsekuensi: Perusahaan kehilangan kepercayaan nasabah karena nasabah mengajukan klaim serta berdampak pada kerugian finansial perusahaan

Berdasarkan konsekuensinya, maka sebisa mungkin membuat model yang dapat mengurangi kerugian perusahaan dengan cara memperbanyak prediksi nasabah yang benar benar mengajukan klaim dan nasabah yang tidak mengajukan klaim. Jadi metric yang akan dipakai adalah Precision Recall Curve karena lebih membutuhkan perhitungan true positif serta terdapat imbalance data.