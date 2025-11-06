# Tugas-Akhir-Judul-2-Jaringan-Komputer

1. Melakukan PING dari PCA ke PCB hasilnya masih RTO
<img width="476" height="184" alt="Screenshot 2025-11-06 161607" src="https://github.com/user-attachments/assets/affb84a3-74ba-4fc9-ab73-e95a460b85ba" />
Berdasarkan gambar tersebut dapat dilihat bahwa terdapat pesan “Request timed out” yang berarti koneksi dari PC-A ke PC-B gagal sepenuhnya (100% packet loss). Hal ini terjadi karena router dan switch belum dikonfigurasi, sehingga perangkat belum memiliki alamat IP, belum mengaktifkan interface, dan belum menjalankan fungsi routing untuk meneruskan paket antarjaringan. Akibatnya, meskipun kabel sudah terpasang secara fisik, lapisan jaringan (Layer 3) belum aktif sehingga data tidak dapat dikirim dari satu subnet ke subnet lain. Setelah router dan switch dikonfigurasi sesuai dengan tabel alamat pada tugas, barulah komunikasi antarperangkat dapat berhasil dilakukan.

2. Melakukan PING dari PCA ke PCB hasilnya Berhasil
<img width="470" height="230" alt="Screenshot 2025-11-06 160902" src="https://github.com/user-attachments/assets/544f00e0-79d7-4b04-86e3-ceb74313c8ec" />
Selanjutnya dapat dilihat bahwa gambar tersebut menunjukkan bahwa koneksi antara PC-A dan PC-B sudah berhasil, ditandai dengan adanya balasan (reply) dari alamat IP 192.168.0.3. Meskipun sempat muncul satu request timed out di awal, hal itu wajar terjadi saat jaringan baru aktif dan perangkat (seperti router atau switch) masih menstabilkan koneksi. Setelah konfigurasi router dan switch selesai dilakukan meliputi pemberian alamat IP, pengaktifan interface, serta pengaturan gateway data dapat dikirim dan diterima dengan baik.

3. Melakukan PING dari S1 ke PCB hasilnya Berhasil
<img width="571" height="106" alt="Screenshot 2025-11-06 160959" src="https://github.com/user-attachments/assets/e8afec36-5952-448f-ac2c-d5735b9af1c3" />
Selanjutnya terdapat ping dari switch S1 ke PC-B (192.168.0.3) yang menunjukkan tingkat keberhasilan 100% (5/5), artinya seluruh paket ICMP berhasil dikirim dan diterima tanpa kehilangan data. Ini menandakan bahwa konfigurasi jaringan sudah benar dan konektivitas antarperangkat berfungsi sempurna. Router telah menjalankan fungsinya sebagai penghubung antarjaringan, semnentara switch berhasil meneruskan lalu lintas data di dalam jaringan lokal. Waktu respons yang sangat rendah (0 ms) menunjukkan bahwa jalur komunikasi antarperangkat berjalan dengan efisien tanpa hambatan.
