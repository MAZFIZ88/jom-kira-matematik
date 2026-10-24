JOM KIRA! MATEMATIK TAHUN 2 — VERSI 4
========================================

KANDUNGAN
- index.html: aplikasi web/PWA dan UI akaun awan
- manifest.json: konfigurasi PWA
- sw.js: cache asas
- supabase_schema.sql: skema pangkalan data dan polisi keselamatan (RLS)
- PANDUAN_AWAL.txt: langkah konfigurasi awan

PENAMBAHBAIKAN VERSI 4
- UI daftar akaun dan log masuk e-mel/kata laluan
- Integrasi Supabase Auth dan PostgreSQL untuk rekod permainan
- Penyegerakan rekod merentas peranti selepas konfigurasi Supabase
- Polisi RLS: murid hanya membaca rekod sendiri; akaun guru boleh membaca rekod murid
- Rekod sedia ada boleh dihantar ke awan selepas log masuk

PENTING
Aplikasi ini BELUM dihoskan dan belum disambungkan kepada projek Supabase sebenar. Pengguna/pentadbir perlu cipta projek sendiri, jalankan supabase_schema.sql, kemudian masukkan Project URL dan anon/publishable key dalam aplikasi. Jangan masukkan service_role key. Untuk PWA, hoskan melalui HTTPS.

BATASAN
- Peranan akaun baharu bermula sebagai murid. Untuk akaun guru, pentadbir perlu menukar role kepada teacher menggunakan arahan SQL dalam PANDUAN_AWAL.txt.
- Ini prototaip: tiada pengurusan kelas/kelas berkod atau reset kata laluan tersuai selain aliran Supabase standard.
- Bank soalan belum disahkan sepenuhnya dengan DSKP KSSR Tahun 2. Semak kandungan sebelum penggunaan rasmi.
- Data markah setempat dan rekod awan digabungkan; jumlah mata pada peranti ialah agregat rekod yang ada di peranti itu.
