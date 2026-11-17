<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flowchart Berangkat Sekolah - Fiona Adinda Melisa</title>
    <!-- Memuat Tailwind CSS untuk tata letak responsif dan palet warna pastel -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Memuat Google Fonts: Poppins & Quicksand untuk nuansa estetik dan jelas dibaca -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700&family=Quicksand:wght@600;700&display=swap" rel="stylesheet">
    <!-- Memuat FontAwesome untuk ikon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #fff5f7; /* Latar belakang pink pastel sangat lembut */
        }
        h1, .font-heading {
            font-family: 'Poppins', sans-serif;
        }
        /* Animasi hover halus pada node SVG flowchart */
        .flow-node {
            transition: transform 0.2s ease, filter 0.2s ease;
            cursor: default;
        }
        .flow-node:hover {
            transform: translateY(-2px);
            filter: drop-shadow(0 6px 12px rgba(244, 114, 182, 0.25));
        }
        /* Pengaturan saat dicetak atau disimpan ke PDF */
        @media print {
            body { background-color: white !important; }
            .no-print { display: none !important; }
            .print-clean { box-shadow: none !important; border: 1.5px solid #f9a8d4 !important; }
        }
    </style>
</head>
<body class="text-rose-950 antialiased min-h-screen py-6 px-4 sm:px-6 lg:px-8">

    <div class="max-w-3xl mx-auto">
        <!-- Header Identitas Siswa Tema Pink Pastel -->
        <div class="bg-gradient-to-r from-pink-200 via-rose-200 to-pink-300 rounded-3xl p-6 sm:p-8 shadow-md border-2 border-pink-300 mb-6 print-clean">
            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between gap-4">
                <div>
                    <span class="inline-block px-3.5 py-1 bg-white/80 text-pink-700 rounded-full text-xs font-bold tracking-wider uppercase mb-2 shadow-xs">
                        <i class="fas fa-heart text-pink-500 mr-1"></i> Tugas Informatika • Flowchart
                    </span>
                    <h1 class="text-2xl sm:text-3xl font-bold text-rose-900 tracking-tight">
                        Flowchart Berangkat Sekolah
                    </h1>
                    <p class="text-rose-800/80 text-sm font-medium mt-1">
                        Diagram alur kegiatan sehari-hari berangkat ke sekolah
                    </p>
                </div>

                <!-- Kartu Identitas Fiona Adinda Melisa -->
                <div class="bg-white/90 backdrop-blur-xs rounded-2xl p-4 border-2 border-pink-300 shadow-xs min-w-[230px]">
                    <div class="text-[11px] text-pink-600 uppercase tracking-wider font-bold">Nama Siswa</div>
                    <div class="font-bold text-base sm:text-lg text-rose-950 leading-tight mt-0.5">
                        Fiona Adinda Melisa
                    </div>
                    <div class="inline-flex items-center gap-1.5 mt-2 px-3 py-0.5 rounded-full bg-pink-100 border border-pink-300 text-pink-800 text-xs font-bold">
                        <i class="fas fa-graduation-cap text-pink-600"></i> Kelas X-3
                    </div>
                </div>
            </div>

            <!-- Tombol Cetak / Simpan PDF -->
            <div class="mt-5 pt-4 border-t border-pink-300/70 flex flex-wrap items-center justify-between gap-3 no-print">
                <span class="text-xs font-semibold text-rose-800 flex items-center gap-1.5">
                    <i class="fas fa-sparkles text-pink-600"></i> Siap dicetak atau disalin ke buku tugas
                </span>
                <button onclick="window.print()" class="inline-flex items-center gap-2 bg-pink-500 hover:bg-pink-600 text-white font-bold text-sm px-4 py-2 rounded-xl shadow-sm transition cursor-pointer">
                    <i class="fas fa-print"></i> Cetak / Simpan PDF
                </button>
            </div>
        </div>

        <!-- Keterangan Simbol Flowchart -->
        <div class="bg-white rounded-2xl p-4 shadow-xs border-2 border-pink-200 mb-6 print-clean">
            <div class="grid grid-cols-2 sm:grid-cols-4 gap-2.5 text-xs">
                <div class="flex items-center gap-2 bg-pink-50 p-2 rounded-xl border border-pink-200">
                    <div class="w-6 h-4 rounded-full bg-pink-300 border border-pink-500 shrink-0"></div>
                    <div>
                        <div class="font-bold text-rose-900">Terminator</div>
                        <div class="text-rose-700 text-[11px]">Mulai / Selesai</div>
                    </div>
                </div>
                <div class="flex items-center gap-2 bg-rose-50 p-2 rounded-xl border border-rose-200">
                    <div class="w-6 h-4 -skew-x-12 bg-rose-200 border border-rose-500 shrink-0"></div>
                    <div>
                        <div class="font-bold text-rose-900">Input / Output</div>
                        <div class="text-rose-700 text-[11px]">Bangun / Sampai</div>
                    </div>
                </div>
                <div class="flex items-center gap-2 bg-pink-50 p-2 rounded-xl border border-pink-200">
                    <div class="w-6 h-4 rounded-xs bg-pink-200 border border-pink-500 shrink-0"></div>
                    <div>
                        <div class="font-bold text-rose-900">Proses</div>
                        <div class="text-rose-700 text-[11px]">Kegiatan</div>
                    </div>
                </div>
                <div class="flex items-center gap-2 bg-rose-50 p-2 rounded-xl border border-rose-200">
                    <div class="w-4 h-4 rotate-45 bg-pink-300 border border-pink-500 shrink-0 ml-1"></div>
                    <div class="ml-1">
                        <div class="font-bold text-rose-900">Decision</div>
                        <div class="text-rose-700 text-[11px]">Pilihan Jalan</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- KANVAS DIAGRAM FLOWCHART SVG (Sesuai Struktur Referensi + Warna Pink Pastel) -->
        <div class="bg-white rounded-3xl p-4 sm:p-8 shadow-md border-2 border-pink-200 print-clean">
            <div class="w-full overflow-x-auto flex justify-center">
                <svg viewBox="0 0 700 840" class="w-full max-w-[660px] h-auto select-none" xmlns="http://www.w3.org/2000/svg">
                    <defs>
                        <!-- Definisi Kepala Panah Pink Pastel Tua -->
                        <marker id="arrow" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
                            <path d="M 0 1.5 L 8.5 5 L 0 8.5 z" fill="#db2777" />
                        </marker>
                        <!-- Bayangan lembut untuk setiap kotak -->
                        <filter id="softShadow" x="-10%" y="-10%" width="120%" height="120%">
                            <feDropShadow dx="0" dy="3" stdDeviation="3" flood-color="#f472b6" flood-opacity="0.18"/>
                        </filter>
                    </defs>

                    <!-- ==================== GARIS KONEKTOR & PANAH ==================== -->
                    <!-- Mulai ke Bangun Tidur -->
                    <line x1="350" y1="80" x2="350" y2="122" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Bangun Tidur ke Mandi -->
                    <line x1="350" y1="185" x2="350" y2="227" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Mandi ke Sarapan -->
                    <line x1="350" y1="285" x2="350" y2="327" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Sarapan ke Belah Ketupat (Pergi Menuju Sekolah) -->
                    <line x1="350" y1="385" x2="350" y2="425" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />

                    <!-- Panah Kiri: Decision ke Bawa Kendaraan Sendiri -->
                    <line x1="270" y1="505" x2="208" y2="505" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Panah Kanan: Decision ke Antar Jemput -->
                    <line x1="430" y1="505" x2="492" y2="505" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />

                    <!-- Jalur Lengkung/Siku dari Bawa Kendaraan Sendiri ke Sampai di Sekolah -->
                    <polyline points="115,535 115,650 245,650" fill="none" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Jalur Lengkung/Siku dari Antar Jemput ke Sampai di Sekolah -->
                    <polyline points="585,535 585,650 455,650" fill="none" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />
                    <!-- Panah Tengah Lurus dari Decision ke Sampai di Sekolah -->
                    <line x1="350" y1="585" x2="350" y2="615" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />

                    <!-- Sampai di Sekolah ke Selesai -->
                    <line x1="350" y1="680" x2="350" y2="725" stroke="#db2777" stroke-width="2.5" marker-end="url(#arrow)" />

                    <!-- ==================== SIMBOL-SIMBOL FLOWCHART ==================== -->

                    <!-- 1. MULAI (Terminator - Kapsul Pink Pastel) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="260" y="25" width="180" height="55" rx="27.5" fill="#fbcfe8" stroke="#ec4899" stroke-width="2.5" />
                        <text x="350" y="58" text-anchor="middle" font-size="16" font-weight="700" fill="#831843">Mulai</text>
                    </g>

                    <!-- 2. BANGUN TIDUR (Input/Output - Jajar Genjang) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <polygon points="270,125 450,125 430,185 250,185" fill="#ffe4e6" stroke="#f43f5e" stroke-width="2.5" stroke-linejoin="round" />
                        <text x="350" y="160" text-anchor="middle" font-size="15" font-weight="700" fill="#881337">Bangun Tidur</text>
                    </g>

                    <!-- 3. MANDI (Proses - Persegi Panjang) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="265" y="230" width="170" height="55" rx="8" fill="#fce7f3" stroke="#ec4899" stroke-width="2.5" />
                        <text x="350" y="263" text-anchor="middle" font-size="15" font-weight="700" fill="#831843">Mandi</text>
                    </g>

                    <!-- 4. SARAPAN (Proses - Persegi Panjang) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="265" y="330" width="170" height="55" rx="8" fill="#fce7f3" stroke="#ec4899" stroke-width="2.5" />
                        <text x="350" y="363" text-anchor="middle" font-size="15" font-weight="700" fill="#831843">Sarapan</text>
                    </g>

                    <!-- 5. PERGI MENUJU SEKOLAH (Decision - Belah Ketupat) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <polygon points="350,428 430,505 350,582 270,505" fill="#fbcfe8" stroke="#db2777" stroke-width="2.5" stroke-linejoin="round" />
                        <text x="350" y="492" text-anchor="middle" font-size="13.5" font-weight="700" fill="#831843">Pergi</text>
                        <text x="350" y="510" text-anchor="middle" font-size="13.5" font-weight="700" fill="#831843">Menuju</text>
                        <text x="350" y="528" text-anchor="middle" font-size="13.5" font-weight="700" fill="#831843">Sekolah</text>
                    </g>

                    <!-- 5A. CABANG KIRI: Bawa Kendaraan Sendiri (Proses) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="25" y="475" width="180" height="60" rx="8" fill="#fff1f2" stroke="#f43f5e" stroke-width="2.5" />
                        <text x="115" y="501" text-anchor="middle" font-size="13.5" font-weight="700" fill="#881337">Bawa Kendaraan</text>
                        <text x="115" y="520" text-anchor="middle" font-size="13.5" font-weight="700" fill="#881337">Sendiri</text>
                    </g>

                    <!-- 5B. CABANG KANAN: Antar Jemput (Proses) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="495" y="475" width="180" height="60" rx="8" fill="#fff1f2" stroke="#f43f5e" stroke-width="2.5" />
                        <text x="585" y="510" text-anchor="middle" font-size="14" font-weight="700" fill="#881337">Antar Jemput</text>
                    </g>

                    <!-- 6. SAMPAI DI SEKOLAH (Input/Output - Jajar Genjang) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <polygon points="265,620 455,620 435,680 245,680" fill="#ffe4e6" stroke="#f43f5e" stroke-width="2.5" stroke-linejoin="round" />
                        <text x="350" y="655" text-anchor="middle" font-size="15" font-weight="700" fill="#881337">Sampai di Sekolah</text>
                    </g>

                    <!-- 7. SELESAI (Terminator - Kapsul Pink Pastel) -->
                    <g class="flow-node" filter="url(#softShadow)">
                        <rect x="260" y="730" width="180" height="60" rx="30" fill="#f9a8d4" stroke="#db2777" stroke-width="2.5" />
                        <text x="350" y="766" text-anchor="middle" font-size="16" font-weight="700" fill="#831843">Selesai</text>
                    </g>
                </svg>
            </div>
        </div>

        <!-- Footer -->
        <div class="text-center text-xs font-semibold text-pink-700/70 mt-5">
            Dibuat khusus untuk <span class="text-pink-800 font-bold">Fiona Adinda Melisa — Kelas X-3</span>
        </div>
    </div>

</body>
</html>
