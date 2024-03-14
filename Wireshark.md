Quality-of-service_Trafic-jaringan-menggunakan-Wireshark
Nama Kelompok:
1.) Habib Hubaddilah
2.) Muh Faisal Bimantara
Yang dibutuhkan

Software Wireshark
Koneksi wifi

Memulai Praktik:

1. Pada bagian ini saya mencoba menjalankan paket data melalui Wireshark dengan Capturing From Wi-Fi seperti gambar di bawah ini. Bagian ini saya memerlukan waktu 10 menit untuk mendapatkan paket data yang sedang berjalan. Seperti Gambar dibawah ini saya mulai pada pukul 09.25

![gmbr wireshark 1](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/b222c89f-c1ae-4f27-b794-2d19f5137d6a)


2. Setelah 10 menit berjalan didapatkan paket data 57553 seperti gambar dibawah ini :

![gmbr wireshark 2](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/79f46ead-e5bd-4c0e-a72d-ef9e1d1c3e88)


3.THROUGHPUT Berikut adalah data yang didapatkan dari paket data yang berjalan pada jarigan Wi-Fi, seperti gambar di bawah ini :

![gmbr wireshark 3](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/89029cdb-b463-4d4b-b1dd-31d76012f4d3)


-Throughput
	  jumlah byte / Time Span = 58717599 Byte /  612,081 s
				= 95931 Bytes/s
				= 95,931 KB/s
				= 95,931 Kb/s x 8
				= 767,448 Kb/s

4. PACKET LOSS Dengan melakukan filtering data, didapatlah beberapa data paket yang tidak terkirim.Berikut adalah data packet loss yang terjadi :

    -Packet Loss 
      	((Paket Dikirim - Paket Diterima)/Paket Dikirim)x100
      	= ((57553 - 56.218)/57553)x 100
      	= (1335/57553)x 100
      	= 2,374684264826212


5. DELAY Convert semua packet tersebut menjadi format CSV dan lakukan analisis data melalui excel. Karna yang diperlukan hanya informasi waktu, maka hilangkan kolum informasi lain pada file csv yang sudah di export

![gmbr wireshark 4](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/0dc365b0-38a2-4cca-8c5a-e758c0494c1f)


Analisis yang didapatkan :

![gmbr wireshark 5](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/6b44a30c-9472-4411-b009-857fc8a43f81)


Time 1 = Waktu awal Time 2 = Waktu awal yang diulai setelah 0 Delay = Time 2 – Time 1

![gmbr wireshark 6](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/79652586-c690-4499-ada0-52733c26f8db)

  -Delay
  total delay : 611,521046
  rata rata delay : 0,010625355


6. JITTER Analisis yang didapatkan adalah : Delay 1 = Nilai Delay – Nilai Delay Setelahnya Delay 2 = Semua Nilai Delay, Kecuali Delay Pertama Jitter = Delay – Delay 1
Jadi, Didapatkan hasil dari nilai jitter dan rata – rata jitter juga didapatkan sebagai berikut

![gmbr wireshark 7](https://github.com/faisalbinta29/TugasWireshark/assets/151717525/44c0d874-f25f-4000-89b4-07098c5d958a)


  -Jitter
  total jiter : 611,463206
  rata rata jitter : 0,01062435
