# README — Tailwind 
- penjelasan desain
 - membuat tampilan profile instagram
  - menggunakan framework tailwind
  - membuat web yang resposive

- jawaban pertanyaan 
 - Keputusan grid-cols/gap
  - mobile 1 kolom biar foto besar dan mudah di-tap
  - sm jadi 2 kolom, md jadi 3 kolom mirip IG desktop
  - gap-1 supaya rapat dan hemat ruang.

- Utility responsive untuk masalah mobile
  - pusatkan dulu: place-items-center text-center
  - di layar lebih besar: sm:grid-cols-[auto,1fr] sm:place-items-start sm:text-left
  - baris tombol/stats: justify-center sm:justify-start
  - highlight biar nggak mepet: overflow-x-auto
  - jaga rasio foto: aspect-square.

- Trade-off utility vs component CSS
  - utility: cepat, konsisten, nggak perlu file CSS, tapi HTML jadi ramai.
  - component CSS: enak dipakai ulang, tapi perlu setup/abstraksi.
  - untuk tugas ini pilih utility murni karena halaman sederhana.
