# Dokumentasi Workshop – Day 1

**Building with AI, Managing Change with GitHub**
| **Nama Lengkap** | Humam Rais Dzaki Hafizhah |
| **Kelas** | TMD 1B – D4 Informatika |
| **Kampus** | Politeknik Negeri Jakarta (PNJ) |

---

## Daftar Isi

1. [Deskripsi Repository](#-deskripsi-repository)
2. [Tujuan Repository](#-tujuan-repository)
3. [Informasi Kegiatan Workshop](#-informasi-kegiatan-workshop)
4. [Rangkuman Materi](#-rangkuman-materi)
   - [Sesi 1 – Building with AI, Managing Change with GitHub](#sesi-1--building-with-ai-managing-change-with-github)
   - [Sesi 2 – Kurikulum Merdeka di Perguruan Tinggi (MBKM & MSIB)](#sesi-2--kurikulum-merdeka-di-perguruan-tinggi-mbkm--msib)
   - [Sesi 3 – Paparan Kurikulum OBE 2026 D4 Teknik Informatika](#sesi-3--paparan-kurikulum-obe-2026-d4-teknik-informatika)
5. [Poin Penting & Pengetahuan Baru](#-poin-penting--pengetahuan-baru)
6. [Pendapat Pribadi tentang Day 1](#-pendapat-pribadi-tentang-day-1)
7. [Referensi](#-referensi)

---

## Deskripsi Repository

Repository ini adalah dokumentasi pribadi saya selama mengikuti **Day 1 Proyek Workshop**. Isinya berupa rangkuman materi yang disampaikan, catatan hal-hal baru yang saya pelajari, dan pendapat saya tentang jalannya kegiatan. Seluruh dokumentasi ditulis dalam satu file `README.md` supaya mudah dibaca langsung di halaman utama repository.

## Tujuan Repository

- Menyimpan dan merapikan catatan materi workshop di satu tempat yang bisa diakses secara daring.
- Melatih saya memakai GitHub untuk menyimpan, mengelola, dan mempublikasikan dokumentasi.
- Membiasakan diri mendokumentasikan hal yang dipelajari, bukan hanya mengikutinya.
- Melatih penulisan catatan terstruktur dengan Markdown (`README.md`).
- Menjadi bahan membaca ulang saya sendiri, dan acuan bagi orang lain yang ingin tahu isi Day 1.

## Informasi Kegiatan Workshop

| Keterangan | Detail |
|---|---|
| **Nama kegiatan** | Proyek Workshop – Day 1 |
| **Tema sesi praktik** | Building with AI, Managing Change with GitHub |
| **Pemateri sesi AI & GitHub** | Nugi Farhan (Senior Product Designer, pengalaman 6 tahun) |
| **Materi pendukung** | Kurikulum Merdeka (MBKM & MSIB); Kurikulum OBE 2026 D4 Teknik Informatika PNJ |
| **Pemateri paparan kurikulum** | Bambang Warsuta, S.Kom., M.T.I. (Kepala Program Studi D4 TI PNJ) |
| **Jenis tugas** | Individu – dokumentasi di repository GitHub Public |

**Capaian yang ditargetkan pada sesi AI & GitHub:**

1. Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
2. Mengidentifikasi *repository*, *commit*, *branch*, dan *pull request*.
3. Membedakan Git dan GitHub.
4. Melakukan *version controlling*.

---

## Rangkuman Materi

### Sesi 1 – Building with AI, Managing Change with GitHub

Sesi ini terdiri dari dua bagian besar: **Prompt Engineering** (cara memberi instruksi ke AI) dan **Git & GitHub** (cara mengelola perubahan kode), lalu ditutup dengan praktik membuat aplikasi sederhana.

#### A. Prompt Engineering

**Apa itu prompt?** Instruksi atau masukan yang kita berikan ke model AI untuk mendapatkan hasil tertentu. Bentuknya bisa pertanyaan sederhana, kata kunci, instruksi yang rumit, atau potongan kode.

**Prompt engineering** adalah cara merancang instruksi agar AI memberi jawaban yang tepat, relevan, dan layak dipakai.

**Context is key.** Prompt tanpa konteks membuat AI menebak-nebak. Prompt yang memuat konteks (siapa penggunanya, batasan teknologinya, hasil yang diharapkan) menghasilkan jawaban yang jauh lebih terarah.

**Struktur prompt yang baik: Role – Task – Context – Format**

| Unsur | Fungsi | Contoh dari materi (Student Task Planner) |
|---|---|---|
| **Role** | Menetapkan peran AI | "Kamu membantu saya membangun aplikasi *student task planner* yang ramah pemula" |
| **Task** | Menjelaskan tujuan dan kebutuhan | Pengelola tugas untuk mahasiswa tahun pertama: daftar tugas, judul, tenggat, status selesai, tombol tandai selesai, filter *all / pending / completed*, tampilan bersih dan responsif |
| **Context** | Memberi batasan dan situasi | Pakai HTML, CSS, dan JavaScript murni; sederhana untuk pemula; tanpa library tambahan; kode rapi dengan penjelasan tiap file |
| **Format** | Menentukan bentuk keluaran | Kode lengkap per file, cara menjalankan, cara menguji interaksi utama, dan AI tidak boleh mengklaim aplikasinya berfungsi sebelum diverifikasi |

**Keuntungan prompt engineering:**
- Meningkatkan performa model AI.
- Mengurangi bias dan respons yang menyinggung.
- Meningkatkan kontrol dan keterprediksian hasil.
- Memberikan pengalaman pengguna yang lebih baik.

#### B. Git dan GitHub

**Apa itu Git?** Sistem *version control* yang mencatat siapa, kapan, dan apa saja yang diubah dalam sebuah file. Git dibuat oleh Linus Torvalds pada 2005.

**Git vs GitHub**

| | Git | GitHub |
|---|---|---|
| **Sifat** | Sistem version control terdistribusi (DVCS) | Platform berbasis web |
| **Fungsi** | Melacak dan mengelola perubahan kode secara lokal | Menyimpan repository Git secara online dan mendukung kolaborasi |

**Tiga area dalam Git workflow**

| Area | Penjelasan |
|---|---|
| **Working directory (working tree)** | Salinan satu versi proyek yang sedang dikerjakan di komputer. Filenya diambil dari database Git. |
| **Staging area (index)** | Tempat menampung perubahan yang akan dimasukkan ke *commit* berikutnya. |
| **Git directory** | Tempat Git menyimpan metadata dan *object database*. Bagian inilah yang disalin saat `git clone`. |

Alurnya: **ubah file** (working directory) → **`git add`** (staging area) → **`git commit`** (tersimpan di repository).

**Perintah dasar Git**

```bash
git init                    # memulai repository baru
git add .                   # memindahkan file ke staging area
git commit -m "pesan"       # menyimpan perubahan ke repository
```

**Perintah menghubungkan ke GitHub**

```bash
git remote add origin <url>   # menghubungkan repo lokal ke repo di GitHub
git push origin main          # mengirim branch saat ini ke remote
git pull origin main          # mengambil perubahan dari remote lalu menggabungkannya
```

**Dua cara memulai repository**
1. Dari lokal: `git init`.
2. Dari GitHub: buat *new repository*, buka tombol **Code**, salin tautannya, lalu `git clone "url"` di terminal.

**Variasi perintah `git add`**

| Perintah | Hasil |
|---|---|
| `git add --all` / `git add -A` | Sama: menambahkan semua perubahan di dalam repository ke staging area |
| `git add .` | Menambahkan semua file di direktori saat ini beserta isinya |
| `git add *` | Menambahkan file yang berubah atau baru, tetapi **tidak** file yang dihapus |

**Persiapan (setup)**

```bash
git --version                                          # cek instalasi, contoh hasil: git version 2.xx.xx
git config --global user.name "Nama Kamu"              # identitas Git
git config --global user.email "email@contoh.com"
git config --global --list                             # cek konfigurasi
```

- **VS Code:** setelah instal, buka Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`), cari **Shell Command: Install 'code' command in PATH**, lalu cek dengan `code --version`.

**Koneksi aman ke GitHub dengan SSH key**

```bash
ssh-keygen -t ed25519 -C "email@domain.com"   # buat SSH key (Enter untuk lokasi default; passphrase opsional)
eval "$(ssh-agent -s)"                        # jalankan SSH agent
ssh-add ~/.ssh/id_ed25519                     # daftarkan key ke agent
# salin isi ~/.ssh/id_ed25519.pub, lalu tempel di
# GitHub → Settings → SSH and GPG keys → New SSH key (Authentication Key)
ssh -T git@github.com                         # uji koneksi
```

Jika berhasil, GitHub membalas bahwa autentikasi sukses tetapi tidak menyediakan akses shell.

> **Catatan:** pada slide, `pbcopy` dan konfigurasi `UseKeychain` / `--apple-use-keychain` khusus **macOS**. Pengguna Windows atau Linux memakai cara menyalin kunci yang berbeda (misalnya `clip` di Windows atau `xclip` di Linux).

**Tentang Ed25519:** "Ed" dari EdDSA (*Edwards-curve Digital Signature Algorithm*), sedangkan "25519" merujuk pada kurva eliptik Curve25519 buatan Daniel J. Bernstein (2011). Singkatnya, skema tanda tangan digital yang aman, cepat, dan tahan terhadap serangan implementasi kriptografi yang umum.

**Checklist setup:** `git --version` → `git config --global user.name` dan `user.email` → `code --version` → `ssh -T git@github.com`.

#### C. Praktik: Student Task Planner

Alur kerja yang dipandu di akhir sesi:

1. Pasang platform AI pendamping (Claude, Antigravity, atau ChatGPT).
2. Tulis prompt untuk membuat aplikasi web.
3. Tambahkan proyek ke Git dengan `git init`.
4. *Commit* dan *push* ke GitHub.
5. Lakukan perubahan pada aplikasi.
6. *Commit* dan *push* lagi.

---

### Sesi 2 – Kurikulum Merdeka di Perguruan Tinggi (MBKM & MSIB)

**MBKM (Merdeka Belajar – Kampus Merdeka)** adalah kebijakan Kemendikbudristek sejak 2020 yang memberi mahasiswa kesempatan mengasah kemampuan sesuai bakat dan minat, termasuk terjun langsung ke dunia kerja.

Tujuan utamanya: lulusan siap kerja dan relevan dengan industri; pembelajaran fleksibel tidak hanya di kelas; kegiatan di luar kampus diakui dan dikonversi menjadi SKS.

| Angka kunci (menurut materi) | Nilai |
|---|---|
| Hak belajar di luar prodi asal | hingga 2 semester* |
| SKS yang dapat diakui per semester | 20 SKS |
| Bentuk kegiatan pembelajaran | 8 bentuk |

**8 bentuk kegiatan MBKM:** pertukaran pelajar, magang/praktik kerja, asistensi mengajar, penelitian/riset, proyek kemanusiaan, kegiatan wirausaha, proyek independen, dan membangun desa/KKN.

**MBKM vs MSIB**

| | MBKM | MSIB |
|---|---|---|
| **Posisi** | Payung kebijakan | Program unggulan, salah satu jalur pelaksanaan MBKM |
| **Isi** | Hak belajar di luar prodi, 8 bentuk kegiatan, konversi SKS | Magang dan Studi Independen Bersertifikat bersama mitra industri |
| **Durasi** | Hingga 2 semester* | 1 semester |

**MSIB terdiri dari dua jalur:**
- **Magang Bersertifikat:** belajar sambil bekerja di mitra, mengerjakan tugas dan proyek nyata, dibimbing mentor industri.
- **Studi Independen Bersertifikat:** belajar kompetensi spesifik dari pakar (short course, bootcamp, atau MOOC) lalu dilanjutkan proyek atau studi kasus.
- Kesamaannya: berdurasi 1 semester, dikonversi 20 SKS, mendapat sertifikat, dan ada peluang rekomendasi ke mitra.

**Skema studi D4 (8 semester):** kuliah di prodi, 1 semester kegiatan MBKM (misalnya MSIB), lalu tugas akhir. Contohnya 1 semester di luar prodi dalam kampus yang sama dan 1 semester di luar kampus seperti magang di industri. Konversi SKS ditetapkan prodi bersama dosen pembimbing, dan susunannya bisa berbeda di tiap prodi.

**Metode pembelajaran yang dibahas**

| Metode | Inti | Hasil |
|---|---|---|
| **Project-Based Learning (PjBL)** | Mengerjakan proyek nyata dalam waktu tertentu, umumnya tim | Produk, prototipe, aplikasi, atau laporan yang dipresentasikan |
| **Problem-Based Learning (PBL)** | Mulai dari masalah nyata yang tidak punya jawaban tunggal; dosen sebagai fasilitator | Solusi hasil analisis mahasiswa |
| **Case-Based Learning (CBL)** | Menganalisis kasus nyata yang sudah tersedia | Rekomendasi solusi beserta alasan dan risikonya |

Langkah CBL: pelajari kasus → identifikasi masalah → analisis dan diskusi → rumuskan solusi → presentasi dan refleksi.

**Manfaat bagi mahasiswa politeknik:** pengalaman kerja nyata, kompetensi yang relevan, jejaring profesional, serta sertifikat dan SKS.

**Alur mengikuti program:**
1. Cek data di PDDikti.
2. Buat akun di portal Kampus Merdeka dan aktifkan lewat email.
3. Pilih program magang atau studi independen.
4. Daftar dan ikuti seleksi.
5. Jalani program, raih sertifikat, ajukan konversi SKS ke prodi.

**Tips sukses:** kenali minat dan arah karier; konsultasi dengan dosen sejak awal; siapkan CV dan portofolio; rapikan data akademik; disiplin mencatat kegiatan harian; dan selalu cek informasi resmi karena ketentuan, kuota, serta mitra bisa berubah tiap periode.

> \* *Slide inti menyebut hak belajar 2 semester, sedangkan slide penutup menyebut 3 semester. Catatan ini mengikuti slide inti. Untuk angka pastinya, rujuk Buku Panduan MBKM resmi.*

---

### Sesi 3 – Paparan Kurikulum OBE 2026 D4 Teknik Informatika

Dipaparkan oleh Kaprodi D4 TI PNJ. Kurikulum memakai pendekatan **Outcome-Based Education (OBE)** dan disusun mundur: dari **profil lulusan → profesi → CPL → mata kuliah**. Lulusan bergelar **S.Tr.Kom** dengan kualifikasi **KKNI level 6**.

**Angka kunci:** 8 semester · 49 mata kuliah · 145 SKS · 11 CPL · 4 profil lulusan.

**Empat profil lulusan** (peran kerja 3–5 tahun setelah lulus):

| Kode | Profil | Contoh profesi |
|---|---|---|
| PL01 | Analis solusi | System Analyst, Business Analyst IT, IT Consultant Junior |
| PL02 | Pengembang aplikasi | Software Developer, Web Developer, Mobile Developer, UI/UX Developer |
| PL03 | Penerap teknologi | Data Analyst Junior, AI/ML Engineer Junior, Cloud Engineer Junior, Network Administrator |
| PL04 | Profesional kolaboratif | IT Project Officer, IT Support Specialist, Technical Writer, Technopreneur |

Profil dirumuskan dari tracer study lulusan 2021–2024, FGD dengan industri (advisory board), SKKNI, benchmark kurikulum, perkembangan IPTEKS, dan Permendiktisaintek No. 39 Tahun 2025.

**Profesi paling fundamental menurut mitra industri:** Data Engineer, AI Engineer, Sales Engineer, dan Consultant.

**11 CPL dan prioritasnya:** CPL 2, 4, 6, 8, dan 11 disorot oleh advisory board. **CPL 6 (komunikasi, kerja sama, dan kepemimpinan dalam tim multidisiplin) adalah yang paling dibutuhkan dunia kerja.** CPL lain tetap penting sebagai penopang.

**Sebaran beban SKS:**

| Semester | SKS | Fokus |
|---|---|---|
| 1–2 | 35 | Dasar: algoritma, struktur data, basis data, matematika |
| 3–4 | 46 | Inti: PBO, rekayasa perangkat lunak, kecerdasan buatan, jaringan, keamanan siber |
| 5–6 | 32 | Pendalaman: big data, pembelajaran mesin, proyek, stream pilihan (KA atau RPL, 9 SKS) |
| 7–8 | 32 | Magang (12 SKS) dan tugas akhir (8 SKS) |

**Belajar yang bertahan lama (Make It Stick).** Paparan ditutup dengan pertanyaan reflektif: apakah cara belajar kita membuat kemampuan bertahan sampai bekerja?

| Mitos | Fakta |
|---|---|
| Membaca ulang berkali-kali cara terbaik | Terasa akrab, belum tentu dikuasai. Menguji diri lebih efektif. |
| Belajar kebut semalam cukup | Materi cepat lupa. Sesi berjarak membuat ingatan bertahan lebih lama. |
| Belajar yang baik harus mulus tanpa salah | Kesulitan yang wajar dan kesalahan memperkuat ingatan jangka panjang. |
| Setiap orang punya satu gaya belajar tetap | Bukti ilmiah tidak mendukung pencocokan gaya belajar. |

**Enam kebiasaan belajar:** uji diri sendiri (*retrieval practice*), beri jeda (*spaced practice*), campur topik (*interleaving*), jelaskan dengan kata sendiri (*elaboration*), coba dulu baru dibahas (*generation*), dan ukur diri secara jujur (*calibration*).

---

## Poin Penting & Pengetahuan Baru

1. **Prompt yang baik punya struktur.** Role–Task–Context–Format membuat hasil AI lebih terarah. Batasan seperti "jangan klaim berhasil sebelum diverifikasi" juga bisa ditulis langsung di prompt.
2. **Git dan GitHub itu berbeda.** Git bekerja lokal untuk melacak perubahan, GitHub menyimpan repository secara online dan mendukung kolaborasi.
3. **Ada tiga area dalam Git:** working directory, staging area, dan Git directory. Karena itu `git add` dan `git commit` adalah dua langkah terpisah.
4. **Alur dasar:** `git init` → `git add` → `git commit` → `git remote add` → `git push`. Untuk repository yang sudah ada di GitHub, mulai dengan `git clone`.
5. **SSH key (Ed25519)** memungkinkan terhubung ke GitHub tanpa memasukkan kata sandi tiap kali, dan bisa diuji dengan `ssh -T git@github.com`.
6. **MBKM adalah payung, MSIB salah satu jalurnya.** Kegiatan di luar kelas bisa dikonversi menjadi SKS (hingga 20 SKS per semester).
7. **PjBL, PBL, dan CBL itu berbeda:** PjBL menghasilkan karya, PBL memecahkan masalah terbuka, CBL menganalisis kasus yang sudah ada.
8. **Kurikulum D4 TI PNJ disusun mundur dari profil lulusan.** Kemampuan kerja sama dan komunikasi (CPL 6) ternyata yang paling dicari industri, bukan hanya kemampuan teknis.
9. **Data Engineer disebut sebagai salah satu profesi fundamental** menurut mitra industri.
10. **Strategi belajar:** menguji diri dan belajar berjarak lebih efektif daripada membaca ulang atau kebut semalam.

---

## Pendapat Pribadi tentang Day 1

> Tulis dengan kata-katamu sendiri. Kerangka di bawah ini tinggal diisi.

Kesan umum tentang Day 1 (padat / bermanfaat / kurang apa):

- *(isi di sini)*

**Yang paling berkesan:**
- *(isi di sini, misalnya soal struktur prompt, Git vs GitHub, MBKM, atau kurikulum)*
- *(isi di sini)*

**Masukan untuk sesi berikutnya:**
- *(isi di sini)*

**Penutup:** *(satu atau dua kalimat tentang apa yang kamu bawa pulang dari Day 1)*

---

## Referensi

- Materi workshop "From AI to GitHub: Building with AI, Managing Change with GitHub" – Nugi Farhan.
- Presentasi "Kurikulum Merdeka di Perguruan Tinggi – MBKM & MSIB". Sumber slide: Kemendikbudristek, Buku Panduan MBKM 2024; portal Kampus Merdeka.
- Paparan "Kurikulum OBE 2026 – Program Studi D4 Teknik Informatika", Politeknik Negeri Jakarta.
- Brown, P. C., Roediger, H. L. III, & McDaniel, M. A. (2014). *Make It Stick: The Science of Successful Learning*. Harvard University Press.
- Google Cloud – [What is prompt engineering?](https://cloud.google.com/discover/what-is-prompt-engineering) (sumber yang dicantumkan di slide).

---

<p align="center"><i>Dokumentasi Day 1 · Humam Rais Dzaki Hafizhah · TMD 1B D4 Informatika</i></p>
# Humam-Rais-Dzaki-Hafizhah
