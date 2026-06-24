# Kel-2-Robot-Delivery-Perpustakaan
Repository ini mendokumentasikan keseluruhan proses pembuatan **Robot Delivery Perpustakaan** (Tema 23), mulai dari tahap pemodelan 3D di komputer hingga proses manufaktur menggunakan mesin *laser cutting* dan perakitan *hardware*.

Proyek ini mendemonstrasikan perancangan robot bergerak (*mobile robot*) berbahan triplek 3 mm dengan sistem penggerak (4 Motor DC Gearbox & 4 Roda), dan sangat cocok bagi yang sedang mempelajari fundamental desain mekanik CAD (*Computer-Aided Design*) dan integrasi aktuator robot.

## Tentang Proyek Ini
Robot ini dirancang khusus untuk memenuhi batasan spesifikasi ketat (dimensi maksimal 300x220x180 mm) dengan fungsionalitas mengangkut buku. Proyek ini membedah alur tersebut secara transparan, menunjukkan bagaimana merancang sambungan material (*interlocking joints*) yang solid dan merakit komponen elektrikal dasar (*Differential Drive*).

## Alur Kerja (Workflow)

### 1. Desain CAD (SolidWorks)
Tahap pemodelan bentuk fisik menggunakan *software* SolidWorks:
* Pembuatan struktur *chassis* bawah sebagai dudukan 4 buah motor gearbox kuning.
* Perancangan sekat dan rak buku di bagian atas bodi robot agar muatan tidak mudah jatuh.
* Penggunaan fitur *Extrude* dan *Cut-Extrude* untuk membuat slot/kait penyambung (*interlocking*) antar bagian bodi.
* Proses *Assembly* digital untuk memastikan tidak ada *part* yang bertabrakan (*interference*) sebelum diproduksi.

### 2. Persiapan Laser Cutting (DXF/SVG)
Tahap persiapan manufaktur di mana model 3D diubah menjadi pola potong 2D:
* *Export* permukaan *part* dari SolidWorks ke format `.DXF` atau `.SVG`.
* Penyesuaian tata letak (*nesting*) pola pada lembaran kerja *software* mesin *laser cutting* untuk menghemat material triplek 3 mm.

### 3. Perakitan Perangkat Keras (*Hardware Assembly*)
Tahap integrasi komponen mekanik dan elektronik di dunia nyata:
* Pemasangan 4 motor DC dan 4 roda penggerak.
* Perakitan kepingan bodi berbahan triplek menggunakan bantuan baut dan mur secukupnya.
* Instalasi baterai dan modul remote kontrol untuk mengaktifkan pergerakan *skid-steer/differential drive*.
