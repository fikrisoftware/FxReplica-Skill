# Recon: replica-skill (Jakeschincariol/replica-skill)

Sumber: https://github.com/Jakeschincariol/replica-skill (README publik, lisensi MIT).
Metode: hanya README publik. Tidak membaca atau menyalin kode sumber, bundle, atau endpoint.
Tidak ada akun, tidak ada screenshot. Semua temuan di bawah berasal dari README; belum diverifikasi langsung di repo.

## Scope

1. Platform: CLI / Claude Code skill pack (bukan aplikasi end-user).
2. Slice: alur inti pipeline, yaitu recon -> architect -> design -> build -> test -> diff.
3. Untuk: tim IT BSS, referensi arsitektur internal. Perlu persetujuan tata kelola TI/legal sebelum dipakai, karena pack ini ditujukan untuk meniru aplikasi pihak ketiga.

## Sumber

| source | URL | yang diberikan |
| --- | --- | --- |
| README repo | https://github.com/Jakeschincariol/replica-skill | daftar 11 skill, alur, file output, lisensi MIT |

## Inventaris "layar" (S = command / antarmuka skill)

ID | screen (skill) | cara akses | tujuan | output utama | states
--- | --- | --- | --- | --- | ---
S01 | replica-recon | `/replica-recon` | peta layar, alur, komponen, model data | recon.md, features.csv | belum dapat dinilai (README)
S02 | replica-architect | `/replica-architect` | stack, skema DB, API | rencana arsitektur | -
S03 | replica-design | `/replica-design` | design system sebagai token | token desain | -
S04 | replica-build | `/replica-build` | bangun layar demi layar | kode aplikasi | -
S05 | replica-backend | `/replica-backend` | auth, DB, pembayaran, integrasi | kode backend | -
S06 | replica-test | `/replica-test` | uji alur, catat bug per severitas | laporan bug | -
S07 | replica-diff | `/replica-diff` | skor parity vs aplikasi asli | skor parity | -
S08 | replica-entrepreneur | `/replica-entrepreneur` | analisis ulasan pengguna, rencana perbaikan | ringkasan ulasan | -
S09 | replica-brand | `/replica-brand` | nama dan merek baru, pindai sisa elemen asli | hasil pindai merek | -
S10 | replica-launch | `/replica-launch` | landing page, harga, listing toko | listing.json | -
S11 | replica-deploy | `/replica-deploy` | preflight lalu rilis ke domain sendiri | status rilis | -

Catatan: tabel ini memakai ID skill, bukan layar aplikasi. Layar aplikasi target belum ada karena target recon ini adalah pack itu sendiri.

## Alur pengguna

F01 Clone aplikasi dari nol
    S01 recon -> S02 architect -> S03 design -> S04 build -> S05 backend -> S06 test -> S07 diff
    edge: sumber publik tidak lengkap; aplikasi target memakai login; merek bentrok (ditangani S09)

F02 Perbaiki produk dari ulasan pengguna
    S08 entrepreneur -> S04 build (ulang layar) -> S06 test -> S07 diff

F03 Rilis ke domain sendiri
    S10 launch -> S11 deploy

Hitungan klik jalur bahagia (F01, per skill): 11 perintah, tidak diukur langsung.

## Komponen

Tidak berlaku. Pack ini tidak punya UI. Komponen yang relevan adalah unit pipeline (skill dan file `replica/*`).

## Model data (inferensi, confidence rendah)

Output antar-skill dibaca dari folder `replica/` di proyek.

```
Recon        recon.md, features.csv
             evidence: README "File output utama"
             confidence: high (nama file), low (isi)
Feature      feature, area, priority, original, clone, notes
             evidence: README, template di recon
             confidence: medium
Listing      listing.json
             evidence: README
             confidence: medium
```

## Yang tidak bisa diclone

Dicatat sebagai `skip` di features.csv:
- Merek, logo, dan aset milik aplikasi asli (dinyatakan pack itu sendiri).
- Layanan jaringan dan penggunanya.
- Konten berlisensi.

## Ukuran

Size: S. Pack kecil (11 skill, markdown). Tidak ada kode aplikasi yang harus dibangun di tahap recon.

Hal sulit: tidak ada, di tahap recon ini. Tahap build/backend nanti bisa M-L.

## Out of scope

- Membaca kode sumber repo target.
- Screenshot, login, atau scraping.
- Penilaian hukum atas peniruan merek.

## Persetujuan

Wajib melalui proses change management dan persetujuan Komite TI BSS sebelum implementasi.

## Next step

`/replica-architect`
