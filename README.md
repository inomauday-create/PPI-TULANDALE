<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PPI Tulandale - Kabupaten Rote Ndao | DKP Provinsi NTT</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .active-tab { border-bottom: 3px solid #2563eb; color: #2563eb; font-weight: bold; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans">

    <!-- Top Bar: Akses & Multi-Akun Terpisah -->
    <header class="bg-blue-950 text-white text-xs py-2.5 px-4 shadow-inner">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-2">
            <div class="flex items-center space-x-2">
                <span class="bg-blue-600 px-2 py-0.5 rounded text-[10px] uppercase font-bold tracking-wider">Resmi</span>
                <span>Dinas Kelautan dan Perikanan Provinsi Nusa Tenggara Timur</span>
            </div>
            <div class="flex items-center space-x-3">
                <!-- Tombol Akun Kontributor / Publik -->
                <button onclick="openModal('modal-auth-tamu')" class="bg-blue-900 hover:bg-blue-800 px-3 py-1.5 rounded transition flex items-center space-x-1.5 border border-blue-800">
                    <i class="fa-solid fa-user-pen text-amber-400"></i>
                    <span>Akun Tamu / Kontributor Berita</span>
                </button>
                <!-- Tombol Login Khusus Pengelola Utama (Admin) -->
                <button onclick="openModal('modal-auth-admin')" class="bg-amber-500 hover:bg-amber-400 text-slate-950 font-bold px-3 py-1.5 rounded transition flex items-center space-x-1.5 shadow-sm">
                    <i class="fa-solid fa-lock text-xs"></i>
                    <span>Login Pengelola Utama</span>
                </button>
            </div>
        </div>
    </header>

    <!-- Navbar Utama -->
    <nav class="sticky top-0 z-40 bg-white/95 backdrop-blur-md shadow-sm border-b border-slate-200">
        <div class="max-w-7xl mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <div class="bg-gradient-to-tr from-blue-700 to-blue-500 text-white p-2.5 rounded-xl font-extrabold text-lg shadow-md">
                    <i class="fa-solid fa-anchor"></i>
                </div>
                <div>
                    <h1 class="font-black text-lg leading-tight text-blue-950 tracking-tight">PPI TULANDALE</h1>
                    <p class="text-[11px] font-medium text-slate-500">Kabupaten Rote Ndao — DKP Prov. NTT</p>
                </div>
            </div>
            <!-- Menu Navigasi Desktop -->
            <div class="hidden lg:flex space-x-6 text-sm font-semibold text-slate-600">
                <a href="#beranda" class="hover:text-blue-600 transition py-1">Beranda</a>
                <a href="#tentang" class="hover:text-blue-600 transition py-1">Tentang Kami</a>
                <a href="#layanan" class="hover:text-blue-600 transition py-1">Layanan</a>
                <a href="#mooc" class="hover:text-blue-600 transition py-1 flex items-center gap-1">MOOC/Pelatihan <span class="bg-emerald-100 text-emerald-800 text-[10px] px-1.5 py-0.5 rounded">Dinamis</span></a>
                <a href="#berita" class="hover:text-blue-600 transition py-1">Berita & Artikel</a>
                <a href="#galeri" class="hover:text-blue-600 transition py-1">Galeri</a>
                <a href="#tim" class="hover:text-blue-600 transition py-1">Tim & Struktur</a>
                <a href="#kontak" class="hover:text-blue-600 transition py-1">Kontak</a>
            </div>
        </div>
    </nav>

    <!-- 🏠 Beranda Section -->
    <section id="beranda" class="relative bg-gradient-to-br from-blue-900 via-blue-900 to-slate-900 text-white py-24 px-4 overflow-hidden">
        <div class="absolute inset-0 opacity-15 bg-[radial-gradient(#60a5fa_1px,transparent_1px)] [background-size:20px_20px]"></div>
        <div class="max-w-7xl mx-auto relative z-10 grid md:grid-cols-2 gap-12 items-center">
            <div>
                <span class="inline-block bg-blue-800/80 border border-blue-700 text-blue-200 text-xs px-3 py-1 rounded-full uppercase tracking-wider font-bold mb-4">
                    <i class="fa-solid fa-water mr-1"></i> Pangkalan Pendaratan Ikan Resmi
                </span>
                <h2 class="text-4xl md:text-5xl font-black mb-6 leading-tight tracking-tight">
                    Pusat Aktivitas Maritim & Perikanan <span class="text-amber-400">Rote Ndao</span>
                </h2>
                <p class="text-slate-300 text-base mb-8 leading-relaxed font-normal">
                    Mengoptimalkan pelayanan bongkar muat kapal, distribusi hasil laut berkualitas, serta tata kelola pelabuhan perikanan yang transparan dan akuntabel di bawah naungan Dinas Kelautan dan Perikanan Provinsi NTT.
                </p>
                <div class="flex flex-wrap gap-4">
                    <a href="#layanan" class="bg-amber-500 text-slate-950 px-6 py-3 rounded-xl font-bold shadow-lg hover:bg-amber-400 transition flex items-center gap-2">
                        <span>Jelajahi Layanan</span> <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <a href="#mooc" class="bg-white/10 hover:bg-white/20 border border-white/20 px-6 py-3 rounded-xl font-bold transition flex items-center gap-2">
                        <span>Ikuti Pelatihan (MOOC)</span>
                    </a>
                </div>
            </div>
            <div class="bg-blue-950/50 border border-blue-800/50 p-6 rounded-3xl backdrop-blur-md shadow-2xl">
                <div class="grid grid-cols-2 gap-4 text-center">
                    <div class="bg-blue-900/40 p-4 rounded-2xl border border-blue-800">
                        <i class="fa-solid fa-ship text-amber-400 text-2xl mb-2"></i>
                        <h4 class="text-2xl font-black">120+</h4>
                        <p class="text-xs text-slate-300 mt-1">Kapal Terdaftar</p>
                    </div>
                    <div class="bg-blue-900/40 p-4 rounded-2xl border border-blue-800">
                        <i class="fa-solid fa-fish text-amber-400 text-2xl mb-2"></i>
                        <h4 class="text-2xl font-black">45 Ton</h4>
                        <p class="text-xs text-slate-300 mt-1">Rata-rata Distribusi/Bulan</p>
                    </div>
                    <div class="bg-blue-900/40 p-4 rounded-2xl border border-blue-800">
                        <i class="fa-solid fa-graduation-cap text-amber-400 text-2xl mb-2"></i>
                        <h4 class="text-2xl font-black">5 Modul</h4>
                        <p class="text-xs text-slate-300 mt-1">Pelatihan Aktif (MOOC)</p>
                    </div>
                    <div class="bg-blue-900/40 p-4 rounded-2xl border border-blue-800">
                        <i class="fa-solid fa-newspaper text-amber-400 text-2xl mb-2"></i>
                        <h4 class="text-2xl font-black">Portal</h4>
                        <p class="text-xs text-slate-300 mt-1">Berita & Kontributor</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 🏢 Tentang Kami Section -->
    <section id="tentang" class="py-20 px-4 max-w-7xl mx-auto">
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div class="bg-slate-200 h-96 rounded-3xl flex flex-col items-center justify-center text-slate-500 font-medium relative overflow-hidden shadow-inner border border-slate-300">
                <i class="fa-solid fa-image text-4xl mb-2 text-slate-400"></i>
                <span>[ Foto Area / Dermaga PPI Tulandale ]</span>
                <div class="absolute bottom-4 left-4 right-4 bg-white/90 backdrop-blur-sm p-4 rounded-2xl text-xs shadow">
                    <p class="font-bold text-blue-950">Pengelola Resmi:</p>
                    <p class="text-slate-600">Dinas Kelautan dan Perikanan Provinsi Nusa Tenggara Timur</p>
                </div>
            </div>
            <div>
                <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-50 px-3 py-1 rounded-full">Profil & Legalitas</span>
                <h3 class="text-3xl font-black text-slate-900 mt-3 mb-4">Tentang PPI Tulandale</h3>
                <p class="text-slate-600 mb-4 leading-relaxed">
                    Pangkalan Pendaratan Ikan (PPI) Tulandale adalah unit pelaksana teknis yang beroperasi di Kabupaten Rote Ndao. Kami menyediakan fasilitas tambat labuh, tempat pemasaran ikan, serta pembinaan nelayan untuk mendongkrak kesejahteraan masyarakat pesisir.
                </p>
                <p class="text-slate-600 mb-6 leading-relaxed">
                    Berada di bawah kendali penuh DKP Provinsi NTT, PPI Tulandale berkomitmen menjalankan standar pelayanan publik yang transparan, aman, dan berdaya saing tinggi.
                </p>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                        <h4 class="font-bold text-blue-950 text-base mb-1"><i class="fa-solid fa-eye text-blue-600 mr-2"></i> Visi</h4>
                        <p class="text-xs text-slate-600 leading-relaxed">Mewujudkan pelabuhan perikanan yang mandiri, produktif, modern, dan berkelanjutan di wilayah terselatan Indonesia.</p>
                    </div>
                    <div class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                        <h4 class="font-bold text-blue-950 text-base mb-1"><i class="fa-solid fa-bullseye text-blue-600 mr-2"></i> Misi</h4>
                        <p class="text-xs text-slate-600 leading-relaxed">Optimalisasi layanan tambat labuh, mutu hasil tangkapan, serta peningkatan kapasitas SDM nelayan melalui edukasi digital.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 🛠️ Layanan / Produk Section -->
    <section id="layanan" class="bg-slate-100 py-20 px-4 border-y border-slate-200">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-100 px-3 py-1 rounded-full">Fasilitas & Jasa</span>
                <h3 class="text-3xl font-black text-slate-900 mt-3">Layanan Unggulan Kami</h3>
                <p class="text-slate-600 text-sm mt-2">Berbagai fasilitas penunjang operasional penangkapan ikan dan administrasi kepelabuhanan.</p>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-200 hover:shadow-md transition">
                    <div class="w-14 h-14 bg-blue-50 text-blue-600 rounded-2xl flex items-center justify-center text-2xl mb-6 shadow-sm"><i class="fa-solid fa-anchor"></i></div>
                    <h4 class="font-bold text-xl mb-3 text-slate-900">Pendaratan & Tambat Labuh</h4>
                    <p class="text-slate-600 text-sm leading-relaxed">Area kolam pelabuhan dan dermaga aman bagi kapal perikanan lokal untuk melakukan aktivitas bongkar muat hasil laut secara teratur.</p>
                </div>
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-200 hover:shadow-md transition">
                    <div class="w-14 h-14 bg-blue-50 text-blue-600 rounded-2xl flex items-center justify-center text-2xl mb-6 shadow-sm"><i class="fa-solid fa-snowflake"></i></div>
                    <h4 class="font-bold text-xl mb-3 text-slate-900">Logistik & Mutu Es</h4>
                    <p class="text-slate-600 text-sm leading-relaxed">Fasilitas pendukung rantai dingin (cold chain) untuk memastikan kualitas dan kesegaran ikan tetap terjaga hingga tiba di tangan pembeli.</p>
                </div>
                <div class="bg-white p-8 rounded-3xl shadow-sm border border-slate-200 hover:shadow-md transition">
                    <div class="w-14 h-14 bg-blue-50 text-blue-600 rounded-2xl flex items-center justify-center text-2xl mb-6 shadow-sm"><i class="fa-solid fa-file-invoice-dollar"></i></div>
                    <h4 class="font-bold text-xl mb-3 text-slate-900">Retribusi & Administrasi</h4>
                    <p class="text-slate-600 text-sm leading-relaxed">Pelayanan pengurusan dokumen kelautan, pelaporan hasil tangkapan, dan pembayaran retribusi daerah secara transparan.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 📚 Bagian Pelatihan Online / MOOC (Dinamis Tambah/Hapus) -->
    <section id="mooc" class="py-20 px-4 max-w-7xl mx-auto">
        <div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-12 gap-4">
            <div>
                <span class="text-xs font-bold text-emerald-700 uppercase tracking-widest bg-emerald-100 px-3 py-1 rounded-full">E-Learning Mandiri</span>
                <h3 class="text-3xl font-black text-slate-900 mt-3">MOOC & Pelatihan Perikanan</h3>
                <p class="text-slate-600 text-sm mt-1">Modul pelatihan digital yang dapat diikuti nelayan, staf, atau publik secara fleksibel.</p>
            </div>
            <div class="flex items-center gap-2">
                <span class="text-xs font-medium text-slate-500 bg-slate-100 px-3 py-1.5 rounded-lg border">Pengelola dapat menambah/menghapus modul via Panel Admin</span>
            </div>
        </div>

        <!-- Daftar Modul Pelatihan (Dinamis / Bisa dikontrol admin) -->
        <div id="mooc-container" class="grid md:grid-cols-3 gap-6">
            <!-- Modul 1 -->
            <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                <div>
                    <div class="h-44 bg-gradient-to-r from-blue-600 to-indigo-600 flex items-center justify-center text-white p-6 relative">
                        <i class="fa-solid fa-book-open-reader text-5xl opacity-80"></i>
                        <span class="absolute top-4 left-4 bg-white/20 backdrop-blur-md text-xs px-2.5 py-1 rounded-full font-semibold">Standar Mutu</span>
                    </div>
                    <div class="p-6">
                        <h4 class="font-bold text-lg mb-2 text-slate-900">Penanganan Ikan Segar di Atas Kapal</h4>
                        <p class="text-xs text-slate-600 leading-relaxed mb-4">Teknik penanganan higienis guna mencegah kerusakan mutu hasil tangkapan sejak dari laut.</p>
                    </div>
                </div>
                <div class="p-6 pt-0">
                    <button onclick="alert('Anda terdaftar dalam modul pelatihan ini. Silakan pelajari materinya.')" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2.5 rounded-xl text-sm transition shadow-sm">
                        Ikuti Pelatihan
                    </button>
                </div>
            </div>
            <!-- Modul 2 -->
            <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                <div>
                    <div class="h-44 bg-gradient-to-r from-emerald-600 to-teal-600 flex items-center justify-center text-white p-6 relative">
                        <i class="fa-solid fa-shield-halved text-5xl opacity-80"></i>
                        <span class="absolute top-4 left-4 bg-white/20 backdrop-blur-md text-xs px-2.5 py-1 rounded-full font-semibold">Keselamatan</span>
                    </div>
                    <div class="p-6">
                        <h4 class="font-bold text-lg mb-2 text-slate-900">Manajemen Keselamatan Kerja Nelayan</h4>
                        <p class="text-xs text-slate-600 leading-relaxed mb-4">Prosedur mitigasi cuaca ekstrem dan penggunaan alat pelindung diri di laut.</p>
                    </div>
                </div>
                <div class="p-6 pt-0">
                    <button onclick="alert('Anda terdaftar dalam modul pelatihan ini. Silakan pelajari materinya.')" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2.5 rounded-xl text-sm transition shadow-sm">
                        Ikuti Pelatihan
                    </button>
                </div>
            </div>
            <!-- Modul 3 -->
            <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                <div>
                    <div class="h-44 bg-gradient-to-r from-amber-600 to-orange-600 flex items-center justify-center text-white p-6 relative">
                        <i class="fa-solid fa-calculator text-5xl opacity-80"></i>
                        <span class="absolute top-4 left-4 bg-white/20 backdrop-blur-md text-xs px-2.5 py-1 rounded-full font-semibold">Administrasi</span>
                    </div>
                    <div class="p-6">
                        <h4 class="font-bold text-lg mb-2 text-slate-900">Pencatatan Logbook & Retribusi Perikanan</h4>
                        <p class="text-xs text-slate-600 leading-relaxed mb-4">Panduan pengisian data tangkapan dan kepatuhan administrasi pelabuhan.</p>
                    </div>
                </div>
                <div class="p-6 pt-0">
                    <button onclick="alert('Anda terdaftar dalam modul pelatihan ini. Silakan pelajari materinya.')" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2.5 rounded-xl text-sm transition shadow-sm">
                        Ikuti Pelatihan
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- 📰 Berita & Artikel Section (Bertindak sebagai Website Berita) -->
    <section id="berita" class="bg-slate-100 py-20 px-4 border-y border-slate-200">
        <div class="max-w-7xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-12 gap-4">
                <div>
                    <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-100 px-3 py-1 rounded-full">Portal Informasi</span>
                    <h3 class="text-3xl font-black text-slate-900 mt-3">Berita & Artikel Terbaru</h3>
                    <p class="text-slate-600 text-sm mt-1">Kabar seputar aktivitas pelabuhan, kebijakan DKP NTT, dan edukasi nelayan.</p>
                </div>
                <button onclick="openModal('modal-auth-tamu')" class="bg-white border border-blue-600 text-blue-600 hover:bg-blue-50 font-bold px-4 py-2.5 rounded-xl text-sm transition shadow-sm flex items-center gap-2">
                    <i class="fa-solid fa-pen-nib"></i> <span>Kirim Tulisan / Berita (Kontributor)</span>
                </button>
            </div>

            <!-- Daftar Artikel / Berita -->
            <div id="berita-container" class="grid md:grid-cols-3 gap-8">
                <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                    <div>
                        <div class="h-48 bg-slate-300 flex items-center justify-center text-slate-400 font-medium">
                            <span>[ Ilustrasi Berita 1 ]</span>
                        </div>
                        <div class="p-6">
                            <div class="flex items-center justify-between text-xs text-slate-400 mb-2">
                                <span><i class="fa-regular fa-calendar mr-1"></i> 26 September 2026</span>
                                <span class="bg-blue-50 text-blue-600 px-2 py-0.5 rounded font-semibold">Aktivitas</span>
                            </div>
                            <h4 class="font-bold text-lg mb-2 text-slate-900">Koordinasi Peningkatan Fasilitas Tambat Labuh di Rote Ndao</h4>
                            <p class="text-xs text-slate-600 leading-relaxed mb-4">Tim Koordinator PPI Tulandale bersama DKP NTT meninjau kesiapan infrastruktur dermaga guna menyambut musim tangkap tahun ini.</p>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <span class="text-xs font-bold text-blue-600 hover:underline cursor-pointer">Baca Selengkapnya &rarr;</span>
                    </div>
                </div>

                <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                    <div>
                        <div class="h-48 bg-slate-300 flex items-center justify-center text-slate-400 font-medium">
                            <span>[ Ilustrasi Berita 2 ]</span>
                        </div>
                        <div class="p-6">
                            <div class="flex items-center justify-between text-xs text-slate-400 mb-2">
                                <span><i class="fa-regular fa-calendar mr-1"></i> 20 September 2026</span>
                                <span class="bg-emerald-50 text-emerald-600 px-2 py-0.5 rounded font-semibold">Edukasi</span>
                            </div>
                            <h4 class="font-bold text-lg mb-2 text-slate-900">Sosialisasi Keselamatan Berlayar dan Cuaca Ekstrem</h4>
                            <p class="text-xs text-slate-600 leading-relaxed mb-4">Pentingnya memantau informasi BMKG sebelum nelayan turun ke laut demi keselamatan pelayaran di perairan Rote Ndao.</p>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <span class="text-xs font-bold text-blue-600 hover:underline cursor-pointer">Baca Selengkapnya &rarr;</span>
                    </div>
                </div>

                <div class="bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between">
                    <div>
                        <div class="h-48 bg-slate-300 flex items-center justify-center text-slate-400 font-medium">
                            <span>[ Ilustrasi Berita 3 ]</span>
                        </div>
                        <div class="p-6">
                            <div class="flex items-center justify-between text-xs text-slate-400 mb-2">
                                <span><i class="fa-regular fa-calendar mr-1"></i> 14 September 2026</span>
                                <span class="bg-amber-50 text-amber-600 px-2 py-0.5 rounded font-semibold">Regulasi</span>
                            </div>
                            <h4 class="font-bold text-lg mb-2 text-slate-900">Penerapan Retribusi Digital Perikanan Tangkap</h4>
                            <p class="text-xs text-slate-600 leading-relaxed mb-4">Peningkatan transparansi pendapatan daerah melalui sistem pembayaran digital bagi pelaku usaha perikanan.</p>
                        </div>
                    </div>
                    <div class="p-6 pt-0">
                        <span class="text-xs font-bold text-blue-600 hover:underline cursor-pointer">Baca Selengkapnya &rarr;</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 🖼️ Galeri Section -->
    <section id="galeri" class="py-20 px-4 max-w-7xl mx-auto">
        <div class="text-center max-w-2xl mx-auto mb-16">
            <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-50 px-3 py-1 rounded-full">Dokumentasi Lapangan</span>
            <h3 class="text-3xl font-black text-slate-900 mt-3">Galeri Kegiatan PPI Tulandale</h3>
            <p class="text-slate-600 text-sm mt-2">Potret aktivitas harian, fasilitas dermaga, dan pelayanan masyarakat.</p>
        </div>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
            <div class="bg-slate-200 h-48 rounded-2xl flex items-center justify-center text-slate-400 text-xs font-medium border border-slate-300">[ Aktivitas Dermaga ]</div>
            <div class="bg-slate-200 h-48 rounded-2xl flex items-center justify-center text-slate-400 text-xs font-medium border border-slate-300">[ Bongkar Muat Ikan ]</div>
            <div class="bg-slate-200 h-48 rounded-2xl flex items-center justify-center text-slate-400 text-xs font-medium border border-slate-300">[ Pertemuan Nelayan ]</div>
            <div class="bg-slate-200 h-48 rounded-2xl flex items-center justify-center text-slate-400 text-xs font-medium border border-slate-300">[ Fasilitas Pelabuhan ]</div>
        </div>
    </section>

    <!-- 👥 Tim & Struktur Perusahaan / Instansi -->
    <section id="tim" class="bg-slate-100 py-20 px-4 border-y border-slate-200">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-100 px-3 py-1 rounded-full">Manajemen Organisasi</span>
                <h3 class="text-3xl font-black text-slate-900 mt-3">Struktur Pengelola PPI Tulandale</h3>
                <p class="text-slate-600 text-sm mt-2">Di bawah pembinaan Dinas Kelautan dan Perikanan Provinsi Nusa Tenggara Timur.</p>
            </div>
            <div class="grid md:grid-cols-3 gap-8 max-w-4xl mx-auto">
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-slate-200 text-center">
                    <div class="w-20 h-20 bg-blue-100 text-blue-600 rounded-full flex items-center justify-center text-2xl mx-auto mb-4 font-bold">DKP</div>
                    <h4 class="font-bold text-lg text-slate-900">Kepala Dinas DKP Prov. NTT</h4>
                    <p class="text-xs text-blue-600 font-semibold mt-1">Pembina Instansi</p>
                </div>
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-slate-200 text-center ring-2 ring-blue-600/50">
                    <div class="w-20 h-20 bg-blue-600 text-white rounded-full flex items-center justify-center text-2xl mx-auto mb-4 font-bold"><i class="fa-solid fa-user-tie"></i></div>
                    <h4 class="font-bold text-lg text-slate-900">Mexkil Blantino Mauday</h4>
                    <p class="text-xs text-blue-600 font-semibold mt-1">Koordinator PPI Tulandale</p>
                </div>
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-slate-200 text-center">
                    <div class="w-20 h-20 bg-slate-100 text-slate-600 rounded-full flex items-center justify-center text-2xl mx-auto mb-4 font-bold"><i class="fa-solid fa-users"></i></div>
                    <h4 class="font-bold text-lg text-slate-900">Tim Operasional & Administrasi</h4>
                    <p class="text-xs text-slate-500 font-semibold mt-1">Staf & Pelayanan Pelabuhan</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 📞 Kontak & Lokasi Section -->
    <section id="kontak" class="py-20 px-4 max-w-7xl mx-auto">
        <div class="grid md:grid-cols-2 gap-12">
            <div>
                <span class="text-xs font-bold text-blue-600 uppercase tracking-widest bg-blue-50 px-3 py-1 rounded-full">Hubungi Kami</span>
                <h3 class="text-3xl font-black text-slate-900 mt-3 mb-4">Informasi Kontak & Lokasi</h3>
                <p class="text-slate-600 text-sm mb-6 leading-relaxed">Silakan hubungi atau kunjungi kantor kami untuk keperluan perizinan, informasi pendaratan ikan, maupun kerja sama.</p>
                
                <div class="space-y-4 text-sm text-slate-700">
                    <div class="flex items-start gap-4 bg-white p-4 rounded-2xl border border-slate-200 shadow-sm">
                        <i class="fa-solid fa-location-dot text-blue-600 text-lg mt-1"></i>
                        <div>
                            <h5 class="font-bold text-slate-900">Alamat Kantor</h5>
                            <p class="text-xs text-slate-600 mt-0.5">Tulandale, Kabupaten Rote Ndao, Nusa Tenggara Timur</p>
                        </div>
                    </div>
                    <div class="flex items-start gap-4 bg-white p-4 rounded-2xl border border-slate-200 shadow-sm">
                        <i class="fa-solid fa-phone text-emerald-600 text-lg mt-1"></i>
                        <div>
                            <h5 class="font-bold text-slate-900">WhatsApp / Telepon</h5>
                            <p class="text-xs text-slate-600 mt-0.5">+62 812-xxxx-xxxx (Layanan Pengaduan & Informasi)</p>
                        </div>
                    </div>
                    <div class="flex items-start gap-4 bg-white p-4 rounded-2xl border border-slate-200 shadow-sm">
                        <i class="fa-solid fa-envelope text-amber-600 text-lg mt-1"></i>
                        <div>
                            <h5 class="font-bold text-slate-900">Email Resmi</h5>
                            <p class="text-xs text-slate-600 mt-0.5">info@ppitulandale.nttprov.go.id</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="bg-slate-200 rounded-3xl h-96 flex items-center justify-center text-slate-500 text-xs font-medium border border-slate-300 shadow-inner">
                <span>[ Integrasi Peta Google Maps — Rote Ndao, NTT ]</span>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-950 text-white py-12 px-4 border-t border-slate-800">
        <div class="max-w-7xl mx-auto grid md:grid-cols-3 gap-8 text-sm">
            <div>
                <h4 class="font-bold text-base mb-3 text-amber-400">PPI Tulandale</h4>
                <p class="text-xs text-slate-400 leading-relaxed">Pangkalan Pendaratan Ikan Tulandale, Kabupaten Rote Ndao. Dikelola di bawah naungan Dinas Kelautan dan Perikanan Provinsi Nusa Tenggara Timur.</p>
            </div>
            <div>
                <h4 class="font-bold text-base mb-3">Tautan Cepat</h4>
                <ul class="text-xs text-slate-400 space-y-2">
                    <li><a href="#beranda" class="hover:text-white">Beranda Utama</a></li>
                    <li><a href="#mooc" class="hover:text-white">Modul Pelatihan Online</a></li>
                    <li><a href="#berita" class="hover:text-white">Portal Berita & Artikel</a></li>
                    <li><a href="#kontak" class="hover:text-white">Kontak & Lokasi</a></li>
                </ul>
            </div>
            <div>
                <h4 class="font-bold text-base mb-3">Legalitas & Sistem</h4>
                <p class="text-xs text-slate-400 leading-relaxed">Dilengkapi sistem multi-pengguna untuk pengelola utama dan kontributor berita serta pelatihan independen.</p>
            </div>
        </div>
        <div class="max-w-7xl mx-auto border-t border-slate-900 mt-8 pt-6 text-center text-xs text-slate-500">
            &copy; 2026 Pangkalan Pendaratan Ikan (PPI) Tulandale — DKP Provinsi NTT. Seluruh Hak Cipta Dilindungi.
        </div>
    </footer>

    <!-- MODAL 1: LOGIN PENGELOLA UTAMA (ADMIN) -->
    <div id="modal-auth-admin" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-md w-full p-6 shadow-2xl relative border border-slate-100">
            <button onclick="closeModal('modal-auth-admin')" class="absolute top-4 right-4 text-slate-400 hover:text-slate-600"><i class="fa-solid fa-xmark text-lg"></i></button>
            <div class="text-center mb-6">
                <div class="w-12 h-12 bg-amber-100 text-amber-600 rounded-2xl flex items-center justify-center text-xl mx-auto mb-2"><i class="fa-solid fa-lock"></i></div>
                <h3 class="font-bold text-xl text-slate-900">Login Pengelola Utama</h3>
                <p class="text-xs text-slate-500 mt-1">Akses khusus admin untuk manajemen pelatihan (MOOC) & moderasi berita.</p>
            </div>
            <form onsubmit="handleAdminLogin(event)" class="space-y-4 text-sm">
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Username / Email Admin</label>
                    <input type="text" id="admin-user" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-4 py-2.5 text-sm focus:outline-none focus:ring-2 focus:ring-blue-600" placeholder="admin@ppitulandale.go.id">
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Kata Sandi</label>
                    <input type="password" id="admin-pass" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-4 py-2.5 text-sm focus:outline-none focus:ring-2 focus:ring-blue-600" placeholder="••••••••">
                </div>
                <button type="submit" class="w-full bg-amber-500 hover:bg-amber-400 text-slate-950 font-bold py-3 rounded-xl transition shadow-sm">Masuk ke Panel Pengelola</button>
            </form>
        </div>
    </div>

    <!-- MODAL 2: AKUN TAMU / KONTRIBUTOR (DAFTAR & KIRIM BERITA / PELATIHAN) -->
    <div id="modal-auth-tamu" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-lg w-full p-6 shadow-2xl relative border border-slate-100 max-h-[90vh] overflow-y-auto">
            <button onclick="closeModal('modal-auth-tamu')" class="absolute top-4 right-4 text-slate-400 hover:text-slate-600"><i class="fa-solid fa-xmark text-lg"></i></button>
            
            <div class="text-center mb-4">
                <div class="w-12 h-12 bg-blue-100 text-blue-600 rounded-2xl flex items-center justify-center text-xl mx-auto mb-2"><i class="fa-solid fa-user-pen"></i></div>
                <h3 class="font-bold text-xl text-slate-900">Portal Akun Tamu & Kontributor</h3>
                <p class="text-xs text-slate-500 mt-1">Kirim tulisan berita atau usulkan modul pelatihan baru.</p>
            </div>

            <!-- Tab Switcher dalam Modal -->
            <div class="flex border-b border-slate-200 mb-4 text-xs font-bold">
                <button onclick="switchTamuTab('form-berita')" id="tab-berita-btn" class="flex-1 pb-2 active-tab">Kirim Berita / Artikel</button>
                <button onclick="switchTamuTab('form-mooc')" id="tab-mooc-btn" class="flex-1 pb-2 text-slate-400">Usulkan Pelatihan MOOC</button>
            </div>

            <!-- Form Kirim Berita -->
            <form id="form-berita" onsubmit="submitBerita(event)" class="space-y-3 text-sm">
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Nama Penulis / Kontributor</label>
                    <input type="text" id="kontributor-nama" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Nama Lengkap Anda">
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Judul Berita / Artikel</label>
                    <input type="text" id="kontributor-judul" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Contoh: Kegiatan Nelayan di Perairan Rote">
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Isi Berita / Artikel</label>
                    <textarea id="kontributor-isi" rows="4" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Tulis berita atau informasi lengkap di sini..."></textarea>
                </div>
                <button type="submit" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2.5 rounded-xl transition shadow-sm text-xs">Kirim Berita ke Pengelola</button>
            </form>

            <!-- Form Usul MOOC -->
            <form id="form-mooc" onsubmit="submitMooc(event)" class="space-y-3 text-sm hidden">
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Nama Pengusul</label>
                    <input type="text" id="mooc-pengusul" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Nama Anda">
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Judul Pelatihan / Modul MOOC</label>
                    <input type="text" id="mooc-judul" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Contoh: Pengolahan Hasil Laut Ekonomis">
                </div>
                <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Deskripsi Singkat Modul</label>
                    <textarea id="mooc-desk" rows="3" required class="w-full bg-slate-50 border border-slate-200 rounded-xl px-3 py-2 text-sm" placeholder="Penjelasan materi pelatihan..."></textarea>
                </div>
                <button type="submit" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-2.5 rounded-xl transition shadow-sm text-xs">Tambah Modul Pelatihan Baru</button>
            </form>
        </div>
    </div>

    <!-- SCRIPT INTERAKTIF & MANAJEMEN KONTEN -->
    <script>
        function openModal(id) {
            document.getElementById(id).classList.remove('hidden');
        }
        function closeModal(id) {
            document.getElementById(id).classList.add('hidden');
        }

        function switchTamuTab(tab) {
            if(tab === 'form-berita') {
                document.getElementById('form-berita').classList.remove('hidden');
                document.getElementById('form-mooc').classList.add('hidden');
                document.getElementById('tab-berita-btn').className = 'flex-1 pb-2 active-tab';
                document.getElementById('tab-mooc-btn').className = 'flex-1 pb-2 text-slate-400';
            } else {
                document.getElementById('form-berita').classList.add('hidden');
                document.getElementById('form-mooc').classList.remove('hidden');
                document.getElementById('tab-mooc-btn').className = 'flex-1 pb-2 active-tab';
                document.getElementById('tab-berita-btn').className = 'flex-1 pb-2 text-slate-400';
            }
        }

        function handleAdminLogin(e) {
            e.preventDefault();
            alert('Login Pengelola Utama Berhasil! Anda sekarang memiliki hak akses penuh untuk mengelola modul dan berita.');
            closeModal('modal-auth-admin');
        }

        // Simulasi Penambahan Berita Kontributor secara Dinamis
        function submitBerita(e) {
            e.preventDefault();
            const nama = document.getElementById('kontributor-nama').value;
            const judul = document.getElementById('kontributor-judul').value;
            const isi = document.getElementById('kontributor-isi').value;

            const container = document.getElementById('berita-container');
            const newCard = document.createElement('div');
            newCard.className = 'bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between';
            newCard.innerHTML = `
                <div>
                    <div class="h-48 bg-blue-100 flex items-center justify-center text-blue-600 font-medium text-xs">
                        <span>[ Kiriman Kontributor: ${nama} ]</span>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center justify-between text-xs text-slate-400 mb-2">
                            <span><i class="fa-regular fa-calendar mr-1"></i> Baru Saja</span>
                            <span class="bg-purple-50 text-purple-600 px-2 py-0.5 rounded font-semibold">Kontributor</span>
                        </div>
                        <h4 class="font-bold text-lg mb-2 text-slate-900">${judul}</h4>
                        <p class="text-xs text-slate-600 leading-relaxed mb-4">${isi}</p>
                    </div>
                </div>
                <div class="p-6 pt-0">
                    <span class="text-xs font-bold text-blue-600 hover:underline cursor-pointer">Baca Selengkapnya &rarr;</span>
                </div>
            `;
            container.prepend(newCard);
            alert('Berita berhasil dikirim dan langsung diterbitkan di portal!');
            closeModal('modal-auth-tamu');
            document.getElementById('form-berita').reset();
        }

        // Simulasi Penambahan Modul MOOC Pelatihan secara Dinamis
        function submitMooc(e) {
            e.preventDefault();
            const judul = document.getElementById('mooc-judul').value;
            const desc = document.getElementById('mooc-desk').value;

            const container = document.getElementById('mooc-container');
            const newMooc = document.createElement('div');
            newMooc.className = 'bg-white rounded-3xl shadow-sm border border-slate-200 overflow-hidden flex flex-col justify-between';
            newMooc.innerHTML = `
                <div>
                    <div class="h-44 bg-gradient-to-r from-purple-600 to-pink-600 flex items-center justify-center text-white p-6 relative">
                        <i class="fa-solid fa-graduation-cap text-5xl opacity-80"></i>
                        <span class="absolute top-4 left-4 bg-white/20 backdrop-blur-md text-xs px-2.5 py-1 rounded-full font-semibold">Pelatihan Baru</span>
                    </div>
                    <div class="p-6">
                        <h4 class="font-bold text-lg mb-2 text-slate-900">${judul}</h4>
                        <p class="text-xs text-slate-600 leading-relaxed mb-4">${desc}</p>
                    </div>
                </div>
                <div class="p-6 pt-0">
                    <button onclick="alert('Anda terdaftar dalam modul pelatihan ini.')" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-2.5 rounded-xl text-sm transition shadow-sm">
                        Ikuti Pelatihan
                    </button>
                </div>
            `;
            container.prepend(newMooc);
            alert('Modul pelatihan MOOC baru berhasil ditambahkan ke daftar!');
            closeModal('modal-auth-tamu');
            document.getElementById('form-mooc').reset();
        }
    </script>
</body>
</html>
