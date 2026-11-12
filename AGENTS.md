# AGENTS.md

## 1. Project Overview

Project ini merupakan aplikasi Personal Finance Management untuk mengelola keuangan pribadi dan rumah tangga.

Tujuan aplikasi:

- Mencatat pemasukan dan pengeluaran.
- Mengelola banyak akun keuangan.
- Mencatat transfer antar-akun.
- Mengelola saldo awal dan saldo akhir.
- Mengelola kategori Needs dan Wants.
- Mengelola beneficiary atau pihak penerima manfaat transaksi.
- Mengelola anggaran bulanan dan tahunan.
- Menyediakan dashboard dan laporan keuangan.
- Menyediakan histori perubahan data keuangan.

Project menggunakan Laravel 13 dan PHP 8.5.

## 2. Technology Stack

Teknologi yang digunakan:

- PHP 8.5.
- Laravel 13.x.
- MySQL 8.x.
- Laravel Blade sebagai frontend.
- Tailwind CSS untuk styling.
- Vanilla JavaScript jika diperlukan.
- Chart.js untuk visualisasi grafik.
- Composer untuk dependency management.
- Vite untuk frontend asset build.
- Git dan GitHub untuk version control.

### Frontend Restrictions

WAJIB menggunakan Laravel Blade.

DILARANG menggunakan:

- Vue.js.
- Inertia.js.
- React.
- SPA terpisah.
- Frontend project terpisah.
- API terpisah khusus untuk frontend.
- Livewire tanpa persetujuan eksplisit.

Gunakan pendekatan server-rendered Laravel dengan Blade dan JavaScript seperlunya.

## 3. Project Scope and Directory Restrictions

Seluruh pekerjaan implementasi harus dibatasi pada root project:

`D:\Data Aldi IT\Keuangan Tahunan\household-finance`

Ketentuan:

1. Jangan membuat, mengubah, menghapus, memindahkan, atau memodifikasi file di luar root project.
2. Jangan mengubah project Laravel lain yang ada di komputer.
3. Jangan mengubah file spreadsheet sumber.
4. Jangan mengubah konfigurasi global Windows, PHP, Composer, Git, atau aplikasi lain tanpa persetujuan.
5. Jangan mengubah konfigurasi global OpenCode.

### 3.1. Project Planning Documents and Reference Materials

Sebelum melakukan analisis, perencanaan, atau implementasi fitur, WAJIB membaca dan memahami dokumen perencanaan yang sudah tersedia di:

`D:\Data Aldi IT\Keuangan Tahunan`

Folder tersebut berisi dokumen dan file hasil perencanaan aplikasi Personal Finance Management yang telah dibuat sebelumnya, termasuk namun tidak terbatas pada:

- Product Requirements Document (PRD).
- System Overview.
- Spreadsheet Analysis.
- Functional Requirements.
- Business Rules.
- Financial Flow.
- System Architecture.
- UI/UX Requirements.
- Development Roadmap.
- Database Review.
- Database Design.
- DBML.
- SQL DDL.
- ERD dalam format Mermaid dan PNG.
- Dokumen pendukung lainnya.

#### Ketentuan Membaca Dokumen

1. Lakukan pemeriksaan struktur folder dan file terlebih dahulu.
2. Identifikasi seluruh dokumen yang relevan dengan tugas.
3. Baca PRD dan dokumen perencanaan terkait sebelum membuat keputusan implementasi.
4. Jangan hanya mengandalkan nama file atau ringkasan dokumen. Baca isi dokumen yang relevan.
5. Gunakan dokumen tersebut sebagai acuan utama kebutuhan produk dan business rules.
6. Jika terdapat beberapa versi dokumen, periksa tanggal, isi, dan statusnya untuk menentukan versi yang paling relevan. Jangan otomatis memilih dokumen terbaru berdasarkan nama file saja.
7. Jangan membuat ulang dokumen yang sudah tersedia tanpa alasan.
8. Jika terdapat informasi yang bertentangan, jangan memilih salah satu secara sepihak. Laporkan perbedaannya dan minta konfirmasi saya.

#### Pemisahan Folder Referensi dan Project

Folder:

`D:\Data Aldi IT\Keuangan Tahunan`

Merupakan lokasi dokumen perencanaan dan referensi.

Sedangkan folder:

`D:\Data Aldi IT\Keuangan Tahunan\household-finance`

Merupakan root project Laravel yang sedang dikembangkan.

**ATURAN PENTING:**

- Folder referensi boleh dibaca.
- Jangan mengubah, menghapus, memindahkan, atau membuat file di folder referensi tanpa persetujuan eksplisit saya.
- Seluruh implementasi kode Laravel hanya boleh dilakukan di dalam root project.
- Jika perlu membuat atau memperbarui dokumentasi selama pengembangan, simpan di dalam folder `docs/` pada root project.
- Jangan menganggap dokumen referensi otomatis boleh dimodifikasi hanya karena dapat dibaca.

#### Prioritas Acuan

Gunakan urutan acuan berikut:

1. Keputusan terbaru yang secara eksplisit saya berikan.
2. PRD yang telah saya setujui.
3. Business Rules dan Financial Flow yang telah disetujui.
4. Database Design yang telah disetujui.
5. Dokumen analisis dan perencanaan lainnya.
6. Pola implementasi dari source code referensi, apabila saya mengizinkan pembacaannya.

Jika belum ada dokumen yang secara resmi disetujui, perlakukan dokumen perencanaan sebagai referensi analisis, bukan izin untuk langsung mengimplementasikannya.

Jangan memulai fitur yang belum tercantum dalam PRD atau belum mendapatkan persetujuan saya.

### Reference Project

Terdapat project lain yang boleh dijadikan referensi apabila saya secara eksplisit meminta Anda membacanya:

`D:\Data Aldi IT\project\be-learning-management-system`

Ketentuannya:

- Project tersebut hanya sebagai referensi pembelajaran pola coding.
- Jangan mengubah file apa pun di sana.
- Jangan menghapus atau membuat file di sana.
- Jangan menjalankan migration, seeder, atau operasi database terhadap project tersebut.
- Jangan menyalin implementasi secara membabi buta.
- Gunakan hanya pola yang relevan dengan kebutuhan project ini.
- Jika perlu membaca project tersebut, pastikan saya sudah mengarahkan atau memberikan izin untuk melakukannya.

Jangan mengakses project lain tanpa arahan saya.

## 4. Development Principles

Prioritaskan:

- Clean Code.
- Readability.
- Maintainability.
- Separation of Concerns.
- Reusability.
- Laravel Best Practices.
- Database Integrity.
- Security.
- Consistent Naming Convention.

Gunakan fitur Laravel bawaan sebelum menambahkan package pihak ketiga.

Jangan menambahkan dependency baru tanpa alasan teknis yang jelas.

Hindari:

- Overengineering.
- Abstraction yang tidak diperlukan.
- Duplikasi business logic.
- Controller yang terlalu besar.
- Query database yang tidak efisien.
- Perubahan besar yang tidak berkaitan dengan tugas.

Jangan melakukan refactor file yang tidak berhubungan dengan permintaan.

## 5. Database Safety Rules

INI MERUPAKAN ATURAN PALING PENTING.

DILARANG melakukan operasi database tanpa instruksi eksplisit dari saya.

### Operasi yang dilarang tanpa persetujuan

Jangan menjalankan:

- `php artisan migrate`
- `php artisan migrate:fresh`
- `php artisan migrate:refresh`
- `php artisan migrate:reset`
- `php artisan db:seed`
- `php artisan db:wipe`
- `php artisan schema:dump`
- SQL `DROP DATABASE`
- SQL `DROP TABLE`
- SQL `TRUNCATE`
- SQL `DELETE` massal
- SQL `UPDATE` massal
- Operasi lain yang dapat mengubah atau menghapus data database.

Jangan melakukan perubahan struktur atau isi database melalui cara lain untuk menghindari aturan ini.

### Migration Rules

Pembuatan file migration hanya boleh dilakukan apabila:

1. Saya secara eksplisit meminta implementasi fitur yang membutuhkan perubahan database.
2. Desain database yang relevan sudah disetujui.
3. Struktur dan dampaknya sudah dianalisis.

Membuat file migration TIDAK berarti mendapatkan izin untuk menjalankannya.

Setiap migration harus:

- Mengikuti desain database yang disetujui.
- Memiliki `up()` dan `down()` yang masuk akal.
- Memperhatikan integritas data.
- Memperhatikan foreign key dan index.
- Menghindari operasi destruktif yang tidak diperlukan.

Sebelum menjalankan migration, wajib meminta persetujuan eksplisit saya.

Jika migration berpotensi menghapus atau mengubah data yang sudah ada, jelaskan risikonya dan tunggu persetujuan khusus.

### Database Environment

Jangan mengasumsikan database yang sedang terhubung adalah database lokal atau database testing.

Sebelum melakukan tindakan database, identifikasi environment dan koneksi yang digunakan.

Jangan pernah mengubah database production tanpa instruksi dan persetujuan khusus.

Jangan mengubah file `.env` tanpa persetujuan saya.

## 6. Git and GitHub Safety Rules

Git digunakan untuk version control, tetapi seluruh tindakan harus mendapat persetujuan sesuai tingkat risikonya.

### Dilarang tanpa instruksi eksplisit

- `git commit`
- `git push`
- `git push --force`
- `git reset --hard`
- `git clean -fd`
- `git rebase`
- `git cherry-pick`
- Menghapus branch.
- Mengubah remote repository.
- Mengubah history commit.
- Menghapus atau menimpa perubahan pengguna.

Jangan melakukan commit atau push secara otomatis setelah menyelesaikan pekerjaan.

### Sebelum Git Operation

Jika saya meminta operasi Git:

1. Periksa branch aktif.
2. Periksa status working tree.
3. Periksa perubahan staged dan unstaged.
4. Periksa file untracked.
5. Identifikasi perubahan yang bukan berasal dari pekerjaan saat ini.
6. Laporkan kondisi repository.
7. Tunggu persetujuan sebelum melakukan tindakan yang mengubah history atau remote.

Jangan memasukkan file `.env`, credential, password, token, API key, atau informasi rahasia ke Git.

Jangan mengubah remote GitHub tanpa persetujuan.

## 7. File Modification Rules

Sebelum mengubah file:

1. Baca file yang relevan secara menyeluruh.
2. Pahami fungsi dan keterkaitannya.
3. Cari pola implementasi yang sudah digunakan.
4. Identifikasi kemungkinan dampak perubahan.
5. Batasi perubahan pada kebutuhan tugas.

Jangan:

- Menghapus file tanpa persetujuan.
- Mengganti isi file secara keseluruhan jika perubahan kecil sudah cukup.
- Mengubah konfigurasi yang tidak relevan.
- Mengubah file yang tidak diminta hanya demi merapikan struktur.
- Menambahkan package atau fitur tambahan tanpa kebutuhan.

Pertahankan kompatibilitas dengan implementasi yang sudah ada.

## 8. Laravel Coding Standards

Gunakan pola Laravel yang sesuai kebutuhan.

### Backend

- Gunakan Form Request untuk validasi yang kompleks atau reusable.
- Gunakan Eloquent ORM untuk interaksi database.
- Gunakan Service Class apabila business logic perlu dipisahkan.
- Gunakan Database Transaction untuk operasi keuangan yang melibatkan beberapa perubahan data.
- Gunakan Policy atau mekanisme authorization Laravel apabila diperlukan.
- Gunakan Laravel Validation.
- Gunakan eager loading untuk mencegah N+1 query.
- Gunakan pagination Laravel untuk daftar data.
- Gunakan exception handling secara konsisten.

Jangan membuat service, repository, interface, atau abstraction hanya untuk mengikuti pola tertentu jika tidak memberikan manfaat nyata.

### Frontend

- Gunakan Blade untuk seluruh halaman.
- Gunakan Blade Components untuk elemen UI yang reusable.
- Gunakan Tailwind CSS.
- Gunakan Vanilla JavaScript untuk interaksi.
- Gunakan Chart.js untuk grafik.
- Pastikan halaman responsive untuk desktop dan mobile.

### Naming Convention

Ikuti konvensi Laravel:

- Model: singular PascalCase.
- Controller: PascalCase dengan akhiran Controller.
- Migration: format bawaan Laravel.
- Table: plural snake_case.
- Column: snake_case.
- Route name: dot notation apabila sesuai.
- Blade view: kebab-case atau mengikuti konvensi folder yang konsisten.

## 9. Financial Business Logic Safety

Semua perhitungan keuangan harus mengikuti business rules dan PRD yang telah disetujui.

Prinsip penting:

- Transfer internal bukan pemasukan atau pengeluaran.
- Biaya transfer merupakan pengeluaran.
- Tabungan direpresentasikan sebagai akun bertipe savings.
- Needs dan Wants merupakan klasifikasi pengeluaran.
- Pemilik akun berbeda konsep dengan beneficiary transaksi.
- Saldo dihitung berdasarkan opening balance dan mutasi transaksi.
- Jangan menyimpan saldo berjalan sebagai sumber kebenaran apabila desain final menggunakan ledger.
- Adjustment saldo harus dibedakan dari income dan expense biasa.
- Opening balance dan rollover tahunan harus konsisten.
- Jangan sampai transfer atau rollover dihitung ganda pada laporan.

Jangan mengubah formula atau business rules tanpa persetujuan.

Jika terdapat ketidaksesuaian antara implementasi dan PRD, laporkan terlebih dahulu.

## 10. Testing and Validation

Setiap perubahan harus divalidasi sesuai ruang lingkup tugas.

Prioritaskan:

- Feature Test.
- Unit Test.
- Validation Test.
- Database Constraint Test.
- Financial Calculation Test.
- Authorization Test.
- Regression Test.

Jangan mengklaim pengujian berhasil apabila belum benar-benar dijalankan.

Jika pengujian tidak dapat dijalankan, jelaskan alasannya.

Jangan menjalankan pengujian yang dapat mengubah database pengguna atau production.

Gunakan database testing yang terisolasi apabila pengujian memerlukan database.

## 11. Required Workflow Before Coding

Untuk setiap tugas implementasi, ikuti tahapan berikut:

### Tahap 1 — Understand

- Baca AGENTS.md.
- Baca PRD dan dokumen terkait.
- Baca file source yang relevan.
- Pahami business rules.
- Identifikasi ruang lingkup tugas.

### Tahap 2 — Analyze

- Identifikasi file yang akan dibuat atau diubah.
- Identifikasi potensi dampak.
- Periksa dependency.
- Periksa risiko database.
- Tentukan strategi implementasi.

### Tahap 3 — Plan

Sampaikan rencana sebelum implementasi apabila tugas melibatkan banyak file, perubahan arsitektur, atau risiko yang signifikan.

Jangan langsung melakukan perubahan besar tanpa penjelasan.

### Tahap 4 — Implement

- Implementasikan hanya permintaan saya.
- Jangan mengerjakan fitur tambahan.
- Jangan melakukan migration atau operasi database tanpa persetujuan.
- Jangan melakukan commit atau push tanpa persetujuan.

### Tahap 5 — Verify

- Periksa hasil perubahan.
- Jalankan test yang aman dan relevan.
- Periksa potensi regression.
- Periksa status Git.
- Pastikan tidak ada perubahan di luar ruang lingkup.

### Tahap 6 — Report

Sampaikan laporan:

1. Ringkasan pekerjaan.
2. File yang dibuat.
3. File yang diubah.
4. Penjelasan implementasi.
5. Pengujian yang dijalankan.
6. Hasil pengujian.
7. Risiko atau catatan.
8. Tindakan yang masih membutuhkan persetujuan.

## 12. Communication Rules

Gunakan bahasa Indonesia dalam penjelasan dan laporan.

Berikan penjelasan teknis secara jelas dan praktis.

Jika ada keputusan yang berpotensi mengubah:

- Struktur database.
- Data keuangan.
- Arsitektur aplikasi.
- Konfigurasi environment.
- Git history atau remote repository.

Berhenti dan minta persetujuan terlebih dahulu.

Jangan membuat asumsi seolah-olah sudah mendapatkan izin.

## 13. Final Priority

Urutan prioritas utama:

1. Keamanan data keuangan.
2. Integritas database.
3. Kesesuaian dengan PRD dan business rules.
4. Keamanan aplikasi.
5. Kualitas implementasi.
6. Maintainability.
7. Performa.
8. Konsistensi UI/UX.

**Prinsip utama: Jangan pernah mengambil tindakan destruktif, mengubah data, menjalankan migration, melakukan commit, atau melakukan push tanpa persetujuan eksplisit dari saya.**
