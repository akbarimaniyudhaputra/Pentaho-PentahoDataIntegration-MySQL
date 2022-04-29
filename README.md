# Pentaho-PentahoDataIntegration-MySQL


## Menghubungkan Pentaho Data Integration dengan MySQL
 - Unduh MySQL Connector : library yang digunakan untuk menghubungkan 2 tools (Pentaho Data Integration dengan MySQL)
 - Setelah terunduh > extract > file berbentuk .jar nya saja copy taruh di folder lib nya Pentaho
 - MySQL Connector saya unduh disini : https://www.softpedia.com/get/Internet/Servers/Database-Utils/MySQL-Connector-J.shtml 
 - Dataset saya unduh disini : https://www.kaggle.com/datasets/fredericobreno/play-tennis


#### Dari file CSV di Pentaho kita simpan ke database di MySQL, dengan cara sebagai berikut :
- 1.) Buat database di MySQL, tablenya kita buat dari CSV file di Pentaho Data Integration
###
![1 0](https://user-images.githubusercontent.com/86678205/166059721-4eea47cf-ceca-43c1-b6fd-1ecc166b7588.PNG)

- 2.) Kita buat transformasi di Pentaho Data Integration
###
![1](https://user-images.githubusercontent.com/86678205/166059806-0d9cc97d-eb07-4c3a-9e26-9603743358a7.png)

- 3.) Membuat koneksi dari Pentaho Data Integration ke MySQL
###
![2](https://user-images.githubusercontent.com/86678205/166059903-d2d546ec-10bb-4f56-b2cb-a6bf898236f2.png)

- 4.) Membuat tab input dan output sumber data CSV ke output table output
###
![3 1](https://user-images.githubusercontent.com/86678205/166059950-c0587127-10d0-4aca-a223-eb8439a4b951.png)
###
![3 2](https://user-images.githubusercontent.com/86678205/166059951-9b80d6d3-7df2-4a04-b646-d7fbb9e432c0.png)

- 5.) Memilih & mendapatkan isi datanya file CSV dari penyimpanan komputer
###
![4 1](https://user-images.githubusercontent.com/86678205/166060016-8aaaf1cd-1f50-436a-ab90-e08fc4122f7d.png)
###
![4 2](https://user-images.githubusercontent.com/86678205/166060067-f6217030-f03e-489c-9fde-1f07459e91ee.png)
###
![4 3](https://user-images.githubusercontent.com/86678205/166060128-c427c942-2c8b-404a-957f-57e9e144ebc9.png)

- 6.) Menambahkan penghubung/hop dari CSV file input ke table output
###
![5 1](https://user-images.githubusercontent.com/86678205/166060150-08b4b182-6860-4394-a0e4-98e0974ff71e.png)
###
![5 2](https://user-images.githubusercontent.com/86678205/166060183-6354e98e-d232-4013-9dff-edc6f37a9d52.png)

- 7.) Atur properties table output
###
![6](https://user-images.githubusercontent.com/86678205/166060215-43c55420-db44-4fe5-8d89-c69b4ec0fb60.png)

- 8.) Save terlebih dahulu file .ktr nya
###

- 9.) Kemudian Run, sukses tidak ada error
###
![7](https://user-images.githubusercontent.com/86678205/166060301-e8453e38-7f5d-486d-aaf4-43f250c60e5d.png)
###
![8](https://user-images.githubusercontent.com/86678205/166060350-f564df05-a39e-445e-88ed-2a38b69ddb2e.png)

- 10.) Cek di MySQL tablenya, refresh terlebih dahulu
###
![9](https://user-images.githubusercontent.com/86678205/166060371-192000cd-4aa1-4144-afae-decc713da668.png)
