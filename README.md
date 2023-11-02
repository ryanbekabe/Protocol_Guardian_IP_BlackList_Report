# Protocol_Guardian_IP_BlackList_Report

git init

git add .

git commit -m "List IP Blocked By Protocol Guardian 102023"

git branch -M main

git push -u origin main


List IP Blocked By Protocol Guardian 092023

Daftar IP yang diblockir oleh Protocol Guardian (v.8f) saat ini meliputi:

1. Blockir dari serangan website menggunakan htaccess, yang proses blocknya berdasarkan ukuran file, jika daftar blockir sudah mencapai byte tertentu, maka IP yang diblockir tersebut sudah boleh kembali mengakses halaman website.

2. Blockir dari serangan SSH Auth menggunakan iptables, yang proses blocknya berdasarkan waktu 1 bulan, jika sudah 1 bulan atau tanggal 1, maka setiap IP yang diblcokir tadi akan dibebaskan kembali untuk mengakses ke server.

Perbedaan dari kedua metode ini adalah, blockir menggunakan htaccess hanya memblock dari mengakses website port 80/443, tapi masih bisa mengakses SSH. Sedangkan blockir menggunakan iptables akan memblock secara keseluruhan baik akses ke website maupun ke SSH.

Pada versi ini, Protocol Guardian hanya memberi keterangan pada notifikasi yang dikirim ke Telegram setiap ada percobaan serangan, baik serangan ke website port 80/443, maupun serangan pada akses SSH. Kedepan insyaa Allah keterangan tersebut akan dilampirkan juga dalam log, sehingga mempermudah dan jelas dalam menganalisa kenapa IP tersebut didaftakan ke blacklist oleh Protocol Guardian.

Protocol Guardian dikembangkan menggunakan Python dan PHP (Apache) untuk saat ini, guna mengamankan server dari serangkaian serangan oleh para Hacker atau Bot Pentest, dan alternatif selain menggunakan CloudFlare. Adapun "Protocol Guardian - IP BlackList Report" ini kumpulan IP yang berhasil dicegat oleh Protocol Guardian dan dipublikasi agar bisa diakses oleh siapa saja yang ingin menggunakan data ini untuk mengamankan servernya dari serangan perangkat-perangkat jahat yang sudah terdaftar selama 1 bulan terakhir ini, maupun sekedar untuk perbandingan data jika sebelumnya sudah memiliki IP Blacklist dan memastikan IP mana yang masih aktif bergerilya melakukan serangan ke server maupun website selama 1 bulan terakhir.

Saat ini program utama Protocol Guardian hanya diterapkan ke beberapa server (VPS) yang menggunakan layanan dari HanyaJasa.Com

Dikembangkan oleh Riyan Hidayat Samosir, S.Kom - HanyaJasa.Com - hanyajasa@gmail.com

