# SIGMA-CNC · Modul Milling

**SI**stem **G**erbang **M**esin **A**mali — Program MPI, Kolej Vokasional Matang

Sistem panduan latihan CNC Milling untuk bengkel Kolej Vokasional Matang.
Satu halaman web tunggal, tiada pemasangan, tiada pangkalan data.

**Laman langsung:** https://mpi-kvmatang.github.io/sigma-cnc/milling/

---

## Apa ini

Laluan tetap tujuh fasa yang membawa pelajar dari persediaan di atas kertas
sehingga bahagian pertama siap diukur. Setiap fasa ada gerbang pemeriksaan
yang mesti lulus sebelum fasa berikut dibenarkan — itulah mekanisme yang
menghalang kesilapan, bukan ingatan pelajar.

Kandungan:

- Aliran kerja bengkel dan kedudukan tiga borang Google sedia ada
- Tangga kompetensi L0 hingga L6 dengan bukti penguasaan setiap aras
- Tujuh fasa Jalan Selamat, lengkap urutan butang panel
- Kalkulator parameter pemotongan (laju spindle, kadar suapan, tinggi sisa)
- Rantai diagnosis untuk enam masalah permukaan yang paling kerap
- Taksonomi sepuluh salah tekan dan pengawal bagi setiap satu
- Rangka pengukuran keberkesanan untuk penilaian projek

## Untuk siapa

Pelajar SVM dan DVM tahun awal yang belum pernah mengendalikan mesin CNC,
serta pensyarah yang menyelia mereka. Mesin sasaran ialah VMC CNC Milling
tiga paksi dengan kawalan FANUC Series 0i-MF Plus.

## Cara guna

Buka pautan laman langsung di atas dalam mana-mana pelayar — telefon,
tablet atau komputer bengkel. Tiada pemasangan diperlukan.

Untuk membukanya tanpa internet, muat turun `milling/index.html` dan klik dua kali.
Halaman berfungsi sepenuhnya secara luar talian; hanya jenis tulisan
bertukar kepada tulisan lalai sistem.

Tiga butang di bahagian atas halaman:

| Butang | Fungsi |
|---|---|
| Tema | Tukar antara auto, cerah dan gelap untuk projektor atau bengkel gelap |
| Reset semua gerbang | Kosongkan semua tanda semak sebelum pelajar berikutnya guna |
| Cetak fasa ini | Cetak fasa semasa sahaja — untuk dilaminate dan digantung di sebelah mesin |

Tanda semak sengaja **tidak** disimpan dalam pelayar. Jika ia kekal, pelajar
seterusnya akan nampak tanda hijau dari semalam dan menyangka gerbang sudah
lulus. Setiap sesi bermula bersih.

## Status

Draf kerja v2.0. Urutan kekunci skrin FANUC sudah disahkan. Butang pada panel
sebelah mesin (pemilih mod, cycle start, feed hold, handwheel) masih bertanda
"Sahkan" kerana ia datang daripada pembuat mesin, bukan FANUC — padankan dengan
manual mesin sebelum diedarkan kepada pelajar.

## Mengubah kandungan

Semua kandungan berada dalam blok `<script>` di hujung `milling/index.html`, sebagai
enam array:

| Array | Kandungan |
|---|---|
| `LEVELS` | Tangga kompetensi L0–L6 |
| `PHASES` | Tujuh fasa: langkah butang, gerbang, kesilapan |
| `SYMPTOMS` | Rantai diagnosis permukaan |
| `TAXO` | Jadual sepuluh salah tekan |
| `MAP` | Pemetaan arketaip A1–A12 |
| `PRESETS` | Bahan untuk kalkulator parameter |

Tukar teks dalam array berkenaan dan halaman terus berubah. Tidak perlu
menyentuh CSS atau HTML.

## Nota keselamatan data

Repositori ini **awam** kerana GitHub Pages memerlukan repositori awam pada
akaun percuma. Jangan sekali-kali memasukkan ke dalam folder ini: nama
pelajar, nombor matrik, jawapan borang, hasil eksport Google Sheets, atau
apa-apa rekod peribadi. Data pelajar kekal di dalam Google Forms yang
dilindungi log masuk.
