# perintah-git
kumpulan perintah-perintah git

Upload project
Di web github, login dan create repository baru sesuai nama aplikasi
Di komputer
cd /var/www/html/aplikasi/
git init
git remote add origin https://github.com/rikyperdana/aplikasi.git
git remote -v
git add .
git commit -m 'Upload pertama'
git push -u origin master
Masukkan username dan password github

Upload pembaharuan
cd /var/www/html/aplikasi/
git status // bakal ditampilkan daftar file yg mengalami perubahan
git add namafile.php // update 1 file ke server
git commit // update semua file ke server
git push origin master // masukkan username dan password
git log // cek perubahan di log

Baca perubahan
cd /var/www/html/aplikasi/
git log

Buat cabang aplikasi
git checkout -b cabangAplikasi
git branch // lihat daftar cabang repo
git push --set-upstream origin cabangAplikasi // usulkan pull request ke master
Buka web github/repo terima confirm pull request dan merge ke master
Delete branch yg sudah disetujui kalau tidak diperlukan lagi
git checkout master // kembali ke repo master
git pull // tarik semua pembaharuan dari server
git branch --delete cabangAplikasi

Kembali ke commit sebelumnya
git reset kode_angka_commit
git reset --hard
