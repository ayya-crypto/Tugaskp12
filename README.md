Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?
State adalah kondisi atau posisi agen saat ini di dalam lingkungan. Pada kasus FrozenLake, state menunjukkan posisi agen pada setiap kotak di peta.
Action adalah tindakan yang dapat dipilih agen untuk berpindah dari satu state ke state lain, seperti bergerak ke atas, bawah, kiri, atau kanan.
Reward adalah nilai umpan balik yang diterima agen setelah melakukan suatu action. Reward digunakan sebagai ukuran keberhasilan tindakan. Pada FrozenLake, agen memperoleh reward 1 jika berhasil mencapai tujuan (goal) dan 0 jika belum berhasil atau gagal.

Apa fungsi dari Learning Rate (α)?
Learning Rate (α) mengatur seberapa besar informasi baru memengaruhi nilai Q yang telah ada. Nilai α = 0,8 pada program berarti agen lebih mengutamakan pengalaman baru dibandingkan pengalaman lama, sehingga proses pembelajaran menjadi lebih cepat, tetapi tetap mempertahankan sebagian informasi sebelumnya.

Apa fungsi dari Discount Factor (γ)?
Discount Factor (γ) menentukan seberapa penting reward di masa depan dibandingkan reward yang diterima saat ini.
Nilai γ = 0,95 membuat agen mempertimbangkan reward jangka panjang, sehingga agen belajar mencari jalur terbaik yang memberikan keuntungan terbesar hingga mencapai tujuan.

Mengapa digunakan metode Exploration dan Exploitation?
Exploration memungkinkan agen mencoba action yang belum pernah dicoba sehingga dapat menemukan jalur atau strategi baru.
Exploitation membuat agen memilih action dengan nilai Q tertinggi berdasarkan pengalaman yang telah dipelajari.
Kombinasi keduanya membantu agen memperoleh pengetahuan yang cukup pada awal pelatihan, kemudian memanfaatkan pengetahuan tersebut untuk mencapai hasil yang optimal.

Bagaimana perubahan nilai reward setelah training 2000 episode?
Berdasarkan kode yang digunakan, reward setiap episode disimpan dan divisualisasikan dalam grafik. Selama proses training, reward pada awal episode umumnya masih rendah karena agen masih banyak melakukan exploration.
Setelah mendekati 2000 episode, reward cenderung meningkat dan menjadi lebih stabil karena nilai epsilon terus menurun sehingga agen lebih banyak melakukan exploitation menggunakan Q-Table yang telah dipelajari.
Hal ini menunjukkan bahwa agen semakin mampu menemukan jalur yang benar menuju goal dan memperoleh reward secara lebih konsisten.
