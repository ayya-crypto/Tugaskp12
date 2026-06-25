1. Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?
  State adalah kondisi atau posisi agen saat ini di dalam lingkungan. Pada kasus FrozenLake, state menunjukkan posisi agen pada setiap kotak di peta.
  Action adalah tindakan yang dapat dipilih agen untuk berpindah dari satu state ke state lain, seperti bergerak ke atas, bawah, kiri, atau kanan.
  Reward adalah nilai umpan balik yang diterima agen setelah melakukan suatu action. Reward digunakan sebagai ukuran keberhasilan tindakan. Pada FrozenLake, agen memperoleh reward 1 jika berhasil mencapai tujuan (goal) dan   0 jika belum berhasil atau gagal.

2. Apa fungsi dari Learning Rate (α)?
  Learning Rate (α) mengatur seberapa besar informasi baru memengaruhi nilai Q yang telah ada. Nilai α = 0,8 pada program berarti agen lebih mengutamakan pengalaman baru dibandingkan pengalaman lama, sehingga proses          pembelajaran menjadi lebih cepat, tetapi tetap mempertahankan sebagian informasi sebelumnya.

3. Apa fungsi dari Discount Factor (γ)?
   Discount Factor (γ) menentukan seberapa penting reward di masa depan dibandingkan reward yang diterima saat ini.
   Nilai γ = 0,95 membuat agen mempertimbangkan reward jangka panjang, sehingga agen belajar mencari jalur terbaik yang memberikan keuntungan terbesar hingga mencapai tujuan.

4. Mengapa digunakan metode Exploration dan Exploitation?
   Exploration memungkinkan agen mencoba action yang belum pernah dicoba sehingga dapat menemukan jalur atau strategi baru.
   Exploitation membuat agen memilih action dengan nilai Q tertinggi berdasarkan pengalaman yang telah dipelajari.
   Kombinasi keduanya membantu agen memperoleh pengetahuan yang cukup pada awal pelatihan, kemudian memanfaatkan pengetahuan tersebut untuk mencapai hasil yang optimal.

5. Bagaimana perubahan nilai reward setelah training 2000 episode?
   Berdasarkan kode yang digunakan, reward setiap episode disimpan dan divisualisasikan dalam grafik. Selama proses training, reward pada awal episode umumnya masih rendah karena agen masih banyak melakukan exploration.
   Setelah mendekati 2000 episode, reward cenderung meningkat dan menjadi lebih stabil karena nilai epsilon terus menurun sehingga agen lebih banyak melakukan exploitation menggunakan Q-Table yang telah dipelajari.
   Hal ini menunjukkan bahwa agen semakin mampu menemukan jalur yang benar menuju goal dan memperoleh reward secara lebih konsisten.

Tugas Lanjutan

Modifikasi program sehingga:
Menggunakan environment Taxi-v3 Menampilkan rata-rata reward setiap 100 episode Membandingkan hasil training 1000, 2000, dan 5000 episode
Hasil 1000
<img width="440" height="392" alt="image" src="https://github.com/user-attachments/assets/2493b7d3-86e5-428b-afab-8f6b9fd01b59" />

Hasil 2000
<img width="551" height="390" alt="image" src="https://github.com/user-attachments/assets/579f6ba2-8af1-4859-9d7c-f954f17f3974" />

Hasil 5000
<img width="515" height="398" alt="image" src="https://github.com/user-attachments/assets/5fe408e4-658f-4867-a3c4-8dcdcad6822a" />
