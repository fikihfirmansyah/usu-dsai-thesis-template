# Template Tesis USU — Program Studi S2 Data Science dan Kecerdasan Buatan

Template LaTeX untuk penulisan tesis Magister (S2) pada Program Studi
Data Science dan Kecerdasan Buatan, Fakultas Ilmu Komputer dan Teknologi
Informasi (Fasilkom-TI), Universitas Sumatera Utara (USU).

Template ini mengikuti aturan format resmi pada:

- **Pedoman Penulisan Tesis**, Fasilkom-TI USU (Cetakan III) — aturan
  kertas, margin, spasi, font, sistematika, dan tata cara sitasi.
- **Overleaf Online LaTeX Editor untuk Penulisan Tesis** — konvensi
  struktur dokumen LaTeX/Overleaf.

## Fitur format yang diimplementasikan

- Kertas A4, font Times New Roman 12pt, spasi 1.5 untuk teks utama
  (spasi tunggal untuk tabel/daftar pustaka).
- Margin naskah: atas 30 mm, kiri 38 mm, kanan 25 mm, bawah 25 mm.
  Margin awal bab (halaman BAB): atas 50 mm.
- Judul bab: "BAB n" lalu judul huruf besar tebal rata tengah.
  Sub-bab level 1: tebal, Title Case. Sub-bab level 2: miring, huruf
  kalimat.
- Penomoran halaman: angka Romawi (bagian muka) lalu angka Arab (bagian
  tubuh dan belakang), diletakkan di kanan atas; tidak dicetak pada
  halaman berjudul (kulit depan, halaman judul, lembar persetujuan,
  daftar isi, dst.) maupun pada halaman awal bab, namun tetap dihitung.
- Sitasi Sistem Pengarang-Tahun (author-year) via `natbib` + `apalike`,
  daftar pustaka disusun alfabetis dengan \textit{hanging indent}.
- Tabel/gambar bernomor per-bab (mis. Tabel 3.1, Gambar 4.1) dengan
  judul tabel di atas dan judul gambar di bawah, rata tengah.

## Struktur berkas

```
main.tex                          - berkas utama (susun semua bagian di sini)
preamble.tex                      - paket dan pengaturan format
frontmatter/
  cover.tex                       - kulit depan (Lampiran 1)
  titlepage.tex                   - halaman judul (Lampiran 4)
  approval.tex                    - lembar persetujuan (Lampiran 5)
  originality.tex                 - pernyataan orisinalitas (Lampiran 6)
  publication.tex                 - persetujuan publikasi (Lampiran 7)
  committee.tex                   - panitia penguji (Lampiran 8)
  cv.tex                          - riwayat hidup (Lampiran 9)
  acknowledgements.tex            - ucapan terima kasih
  abstract_id.tex                 - abstrak Bahasa Indonesia (Lampiran 10)
  abstract_en.tex                 - abstract Bahasa Inggris (Lampiran 11)
chapters/
  bab1_pendahuluan.tex
  bab2_tinjauan_pustaka.tex
  bab3_metodologi.tex
  bab4_hasil_pembahasan.tex
  bab5_kesimpulan_saran.tex
appendix/
  lampiranA_kode_program.tex
  lampiranB_data_tambahan.tex
figures/                          - simpan gambar Anda di sini
references.bib                    - basis data pustaka (BibTeX)
```

## Cara penggunaan

1. Salin (clone) template ini di Overleaf.
2. Ganti seluruh isi contoh pada `frontmatter/` (judul, nama, NIM,
   pembimbing, penguji, riwayat hidup, abstrak) dengan data Anda.
3. Ganti `\ThesisLogo` pada `preamble.tex` dengan
   `\includegraphics[width=50mm,height=50mm]{figures/logo.png}` setelah
   Anda memiliki berkas logo resmi Fasilkom-TI/USU.
4. Tulis isi bab pada `chapters/`, tambahkan gambar ke `figures/`, dan
   kelola pustaka pada `references.bib`.
5. Kompilasi dengan pdfLaTeX + BibTeX (atau mesin \texttt{pdflatex →
   bibtex → pdflatex → pdflatex} pada Overleaf).

## Kesesuaian dengan Overleaf Template Gallery

Template ini adalah **template resmi universitas** untuk penulisan
tesis pada Program Studi S2 Data Science dan Kecerdasan Buatan,
Fasilkom-TI, Universitas Sumatera Utara, dan menautkan ke pedoman resmi
program studi sebagai sumber aturan format. Seluruh isi contoh
menggunakan teks/data isian (\textit{placeholder}), tanpa data pribadi
sungguhan, sesuai kebijakan galeri Overleaf.

## Lisensi

Dirilis di bawah [LaTeX Project Public License](https://www.latex-project.org/lppl/) (LPPL) versi 1.3c atau yang lebih baru.
