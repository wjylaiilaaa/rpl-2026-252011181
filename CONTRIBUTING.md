# Panduan Kontribusi

Repository ini digunakan untuk menyimpan tugas dan dokumentasi pembelajaran mata kuliah Rekayasa Perangkat Lunak (RPL). Panduan ini dibuat agar pengelolaan file dan setiap perubahan yang dilakukan dapat berjalan secara teratur, jelas, dan mudah ditelusuri.

---

## 1. Ketentuan Kontribusi

Perubahan yang dilakukan harus sesuai dengan tujuan repository, seperti menambahkan materi, memperbaiki kesalahan, atau menyempurnakan dokumentasi.

Sebelum melakukan perubahan, pastikan isi file sudah diperiksa dan perubahan yang dibuat tidak menghilangkan informasi penting.

## 2. Penggunaan Branch

Gunakan branch terpisah untuk setiap pekerjaan agar perubahan dapat diperiksa sebelum diterapkan ke branch utama.

| Branch | Keterangan |
|---|---|
| `main` | Menyimpan versi utama repository |
| `docs/nama-dokumen` | Memperbarui dokumentasi |
| `fix/nama-perbaikan` | Memperbaiki kesalahan |
| `feature/nama-fitur` | Menambahkan fitur atau konten baru |

Contoh membuat branch baru:

```bash
git switch main
git pull origin main
git switch -c docs/perbaikan-laporan
```

Hindari melakukan perubahan langsung pada `main` ketika sedang mengerjakan tugas baru.

## 3. Format Commit

Setiap perubahan perlu dicatat menggunakan pesan commit yang singkat dan menggambarkan pekerjaan yang dilakukan.

Format pesan commit:

`jenis: deskripsi perubahan`

Contoh penggunaan:

| Jenis | Contoh Pesan |
|---|---|
| `docs` | `docs: update README` |
| `feat` | `feat: add learning material` |
| `fix` | `fix: correct spelling errors` |
| `refactor` | `refactor: reorganize files` |

Contoh perintah untuk menyimpan perubahan:

```bash
git add .
git commit -m "docs: update project documentation"
```

Usahakan setiap commit berisi perubahan yang saling berkaitan agar riwayat pekerjaan lebih mudah dipahami.

## 4. Pull Request dan Review

Pull Request (PR) digunakan untuk mengajukan perubahan agar dapat diperiksa sebelum digabungkan ke branch utama.

Tahapan yang perlu dilakukan:

1. Buat branch sesuai dengan pekerjaan.
2. Lakukan perubahan pada file yang diperlukan.
3. Periksa kembali isi file dan hasil perubahan.
4. Simpan perubahan melalui commit.
5. Unggah branch ke GitHub.
6. Ajukan Pull Request menuju branch `main`.
7. Lakukan pemeriksaan sebelum perubahan digabungkan.

Untuk mengunggah branch, gunakan perintah:

```bash
git push -u origin docs/perbaikan-laporan
```

Jika repository dikerjakan bersama, mintalah anggota lain untuk meninjau perubahan. Jika dikerjakan secara individu, lakukan pemeriksaan mandiri sebelum melakukan merge.

## 5. Pemeriksaan Sebelum Merge

Sebelum perubahan diterapkan ke branch utama, pastikan hal-hal berikut sudah terpenuhi:

- [ ] Perubahan sesuai dengan tujuan pengerjaan.
- [ ] Tidak terdapat kesalahan penulisan atau format yang diketahui.
- [ ] File yang diperbarui telah diperiksa.
- [ ] Pesan commit menjelaskan perubahan dengan jelas.
- [ ] Dokumentasi telah disesuaikan jika diperlukan.
- [ ] Tidak ada informasi rahasia yang ikut terunggah.

Apabila ditemukan masalah, lakukan perbaikan terlebih dahulu sebelum perubahan digabungkan.

## 6. Penanganan Revisi

Setiap kesalahan atau masukan yang ditemukan selama proses pengerjaan perlu ditindaklanjuti dengan perbaikan yang sesuai.

Perubahan harus dilakukan secara hati-hati agar tidak memengaruhi bagian lain yang masih digunakan. Jika terdapat perubahan kebutuhan, pastikan hasil akhirnya tetap sesuai dengan tujuan repository.

## 7. Etika Kontribusi

Setiap kontributor diharapkan menjaga kualitas pekerjaan dan menghargai kontribusi pihak lain. Referensi yang digunakan perlu dicantumkan dengan semestinya, dan hasil pekerjaan orang lain tidak boleh diakui sebagai hasil pribadi.

Selain itu, komunikasi harus tetap sopan, informasi sensitif harus dijaga, dan setiap masukan perlu disikapi secara terbuka untuk mendukung perbaikan hasil pekerjaan.

---

## Penutup

Panduan ini menjadi acuan dalam mengelola perubahan repository agar lebih terstruktur dan mudah ditinjau. Penggunaan branch yang tepat, pesan commit yang jelas, serta pemeriksaan sebelum merge merupakan bagian penting dalam membangun kebiasaan pengembangan perangkat lunak yang baik.
