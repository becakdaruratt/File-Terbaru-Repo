# File-Terbaru-Repo
git remote -> untuk melihat nama dari remote (secara default namanya origin)
git remote -v -> untuk melihat remote secara detail
git config --list -> untuk melihat id dan email yang kita hbuungkna
git clone (HTTPS) -> untuk menghubungkan dan mengclone , github kita ke git local
git push -> untuk mengirim perubahan commit ke repo github , karena jika kita commit di local komputer kita yang terjadi adalah commitnya maju 1 langkah ,
setelah kita push , mungkin teman teamn di minta id dan password untuk pertama kali , maka secara otomatis file yang kita commit akan bertambah di github kita , dan biasanya id password kita tersimpan di sistem kita, jadi tidak perlu login kembali tapi mungkin suatu saat di minta lagi itu , jika kita menggunakan HTTPS , sedangkan kalau menggunakan SSH tidak perlu menggunakan login seperti itu , harus kita git push kan dahulu barulah di github nya itu bisa sama

    Ctt: setiap kali di bikin commit , github akan selalu ketinggalan 1 commit

    jadi kalau kita lihat kita sudah mengambil repo dari github kita ke local dekstop kita , dengan cara mencopy link dari HTTPS dari github kita dan klik dekstop klik kanan , pilih git bash dan mengetik git clone (link HTTP) , jadi secara otomatis kita sudah mengkloning file dari repo github kita ke local kita, perlu kita perhatikan kalau , kita sebenarnya belum masuk ke , folder git kita kalau kita lihat ls (list semua file) masih memperlihatkan semua daftar file yang ada di dekstop kita , dan ketika ktia mengkoling sebuah repo dari github itu otomatis di buatkan nama dari remotnya , dan sebenarnya nama dari remotenya bisa kita bisa bikin sendiri dan itu bebes , setelah kita ketik di git bashnya git remote -v , kita bisa melihat ada 2 folder , ada fetch dan push , dengan alamat yang sama , kalau kita git status kita akan di berikan pesan yang berbeda dengan yang sebelumnya , biasanya kita di kasih tau on branch , tapi skarang kita di kasih tau your branch  is up to date with 'origin/maser'. (branch yang kita punya di lokal itu sudah sama dengan branch yang ada di repo kita) , ini yang kita ingin kan , setiap ada perubahan kita ingin kedua branch antara local dengna github nya itu sama , pada saat kita lihat visualiasai nya ,dengan git log --all --decorate --oneline --graph , kita bisa melihat , sebuah commit yang di dalamnya ada 3 buah branch , yang warna merah itu adalah branch yang kita punya , dan berada di github kita , namanya origin , dan sekarang semuanya berada di pointer yang sama , artinya up to date lah istilahnya , skarang gini ceritanya di local kita , kita mau menambahkan dan mengubah sesuatu, misalnya kita menambahkan file baru , kita buat misalkan index.html atau file baru bebas lah , 
    aritnya branch kita mendahului , 1 commit dengan yang ada di github kita , jadi saat kita lihat secara visual , kita bisa lihat , kalau branch origin nya sudah tidak sama dengan master , dari gitnya , dan supaya perubahannya sama , kita harus kirim perubahannya ke remote kita , dengan menggunakan kalimat perintah push