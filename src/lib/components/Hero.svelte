<script lang="ts">
    // Hero component for Kawalharta
</script>

<section class="flex flex-col items-center pt-10 pb-20 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto">
    <!-- Top Pill -->
    <div class="flex items-center gap-2 bg-white border border-gray-200 rounded-full pl-1 pr-2 py-1 shadow-sm mb-4 hover:border-gray-300 transition-colors cursor-pointer">
        <span class="bg-black text-white text-[10px] font-bold px-1.5 py-0.5 rounded-full tracking-wide">LIVE</span>
        <span class="text-xs font-medium text-gray-600">690 officials tracked</span>
        <svg viewBox="0 0 16 16" fill="currentColor" class="w-3.5 h-3.5 text-gray-400"><path fill-rule="evenodd" d="M6.22 4.22a.75.75 0 0 1 1.06 0l3.25 3.25a.75.75 0 0 1 0 1.06l-3.25 3.25a.75.75 0 0 1-1.06-1.06L8.94 8 6.22 5.28a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" /></svg>
    </div>

    <!-- Tagline Badge -->
    <div class="bg-gray-50 border border-gray-200 text-gray-700 text-sm font-medium px-4 py-1.5 rounded-full flex items-center gap-2 mb-10 shadow-sm">
        <span class="text-base">🇮🇩</span>
        Transparansi membangun kepercayaan
    </div>

    <!-- Headline -->
    <h1 class="text-5xl sm:text-6xl md:text-7xl font-bold text-center tracking-tight text-gray-900 mb-6 max-w-4xl leading-[1.1]">
        Track Indonesian<br />
        official wealth changes
    </h1>

    <!-- Subheadline -->
    <p class="text-lg sm:text-xl text-gray-500 text-center max-w-2xl mb-16 leading-relaxed">
        Automated LHKPN data aggregation and visualization. Monitor 690 officials across 15+ government institutions tracking Rp 44.7 trillion in assets.
    </p>

    <!-- Hero Image / Mock Interface -->
    <div class="w-full relative">
        <!-- Background Glow Effects -->
        <div class="absolute -left-20 top-20 w-96 h-96 bg-primary-200/30 rounded-full blur-3xl mix-blend-multiply filter opacity-70 animate-blob pointer-events-none"></div>
        <div class="absolute -right-20 top-40 w-96 h-96 bg-primary-300/20 rounded-full blur-3xl mix-blend-multiply filter opacity-70 animate-blob animation-delay-2000 pointer-events-none"></div>

        <!-- Dashboard Preview -->
        <div class="rounded-xl border border-gray-200 bg-white shadow-2xl overflow-hidden relative z-10">
            <div class="flex h-[600px]">
                <!-- Sidebar -->
                <div class="w-64 bg-gray-50 border-r border-gray-200 p-4">
                    <div class="flex items-center gap-2 font-bold text-gray-900 mb-6">
                        <span class="text-xl">🇮🇩</span>
                        Kawalharta
                    </div>
                    <div class="bg-white border border-gray-200 rounded-lg p-3 mb-4">
                        <div class="text-xs text-gray-500">Total Aset</div>
                        <div class="text-xl font-bold text-gray-900">Rp 44.7 T</div>
                    </div>
                    <div class="space-y-2 text-sm">
                        <div class="px-3 py-2 bg-gray-200 rounded-md font-medium text-gray-900">Beranda</div>
                        <div class="px-3 py-2 text-gray-600">Perubahan Terbaru</div>
                        <div class="px-3 py-2 text-gray-600 flex items-center justify-between">
                            <span>Watchlist</span>
                            <span class="bg-primary-600 text-white text-xs px-2 py-0.5 rounded-full">4</span>
                        </div>
                    </div>
                    <div class="mt-6">
                        <div class="text-xs text-gray-400 mb-2">Institusi</div>
                        <div class="space-y-2 text-sm text-gray-600">
                            <div class="flex items-center justify-between px-2">
                                <span>🏛️ DPR RI</span>
                                <span class="text-xs">142</span>
                            </div>
                            <div class="flex items-center justify-between px-2">
                                <span>🏢 Kementerian</span>
                                <span class="text-xs">234</span>
                            </div>
                            <div class="flex items-center justify-between px-2">
                                <span>🏙️ Pemda</span>
                                <span class="text-xs">156</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Main Content -->
                <div class="flex-1 p-6 bg-white">
                    <h2 class="text-2xl font-bold text-gray-900 mb-6">Perubahan Harta Terbaru</h2>
                    <div class="space-y-3">
                        <!-- Official 1 -->
                        <div class="flex items-center gap-4 p-4 border border-gray-200 rounded-lg hover:bg-gray-50">
                            <div class="w-10 h-10 rounded-full bg-gray-200 flex items-center justify-center font-bold text-sm text-gray-600">
                                AB
                            </div>
                            <div class="flex-1">
                                <div class="font-semibold text-gray-900">Anies Baswedan</div>
                                <div class="text-sm text-gray-600">Menteri Pendidikan</div>
                                <div class="text-xs text-gray-500 mt-1">🏢 Kementerian • 2 hari lalu</div>
                            </div>
                            <div class="text-sm font-bold text-green-600">+Rp 2.4 M</div>
                        </div>

                        <!-- Official 2 -->
                        <div class="flex items-center gap-4 p-4 border border-gray-200 rounded-lg hover:bg-gray-50">
                            <div class="w-10 h-10 rounded-full bg-gray-200 flex items-center justify-center font-bold text-sm text-gray-600">
                                PS
                            </div>
                            <div class="flex-1">
                                <div class="font-semibold text-gray-900">Prabowo Subianto</div>
                                <div class="text-sm text-gray-600">Presiden RI</div>
                                <div class="text-xs text-gray-500 mt-1">⚖️ Lembaga Negara • 3 hari lalu</div>
                            </div>
                            <div class="text-sm font-bold text-green-600">+Rp 15.8 M</div>
                        </div>

                        <!-- Official 3 -->
                        <div class="flex items-center gap-4 p-4 border border-gray-200 rounded-lg hover:bg-gray-50">
                            <div class="w-10 h-10 rounded-full bg-gray-200 flex items-center justify-center font-bold text-sm text-gray-600">
                                GP
                            </div>
                            <div class="flex-1">
                                <div class="font-semibold text-gray-900">Ganjar Pranowo</div>
                                <div class="text-sm text-gray-600">Gubernur Jawa Tengah</div>
                                <div class="text-xs text-gray-500 mt-1">🏙️ Pemerintah Daerah • 5 hari lalu</div>
                            </div>
                            <div class="text-sm font-bold text-red-600">-Rp 890 Jt</div>
                        </div>

                        <!-- Official 4 -->
                        <div class="flex items-center gap-4 p-4 border border-gray-200 rounded-lg hover:bg-gray-50">
                            <div class="w-10 h-10 rounded-full bg-gray-200 flex items-center justify-center font-bold text-sm text-gray-600">
                                RK
                            </div>
                            <div class="flex-1">
                                <div class="font-semibold text-gray-900">Ridwan Kamil</div>
                                <div class="text-sm text-gray-600">Gubernur Jawa Barat</div>
                                <div class="text-xs text-gray-500 mt-1">🏙️ Pemerintah Daerah • 1 minggu lalu</div>
                            </div>
                            <div class="text-sm font-bold text-green-600">+Rp 3.2 M</div>
                        </div>
                    </div>
                </div>

                <!-- Right Sidebar -->
                <div class="w-64 border-l border-gray-200 bg-gray-50 p-4">
                    <div class="text-sm font-semibold text-gray-900 mb-4">Watchlist Saya</div>
                    <div class="space-y-3 mb-6">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 rounded-full bg-gray-200 flex items-center justify-center text-xs font-bold text-gray-600">AB</div>
                            <div class="flex-1 min-w-0">
                                <div class="text-sm font-medium text-gray-900 truncate">Anies Baswedan</div>
                                <div class="text-xs text-green-600 flex items-center gap-1">
                                    <div class="w-1.5 h-1.5 bg-green-500 rounded-full"></div>
                                    Alert aktif
                                </div>
                            </div>
                        </div>
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 rounded-full bg-gray-200 flex items-center justify-center text-xs font-bold text-gray-600">PS</div>
                            <div class="flex-1 min-w-0">
                                <div class="text-sm font-medium text-gray-900 truncate">Prabowo Subianto</div>
                                <div class="text-xs text-green-600 flex items-center gap-1">
                                    <div class="w-1.5 h-1.5 bg-green-500 rounded-full"></div>
                                    Alert aktif
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="bg-primary-50 border border-primary-200 rounded-lg p-3">
                        <div class="text-xs font-semibold text-gray-900 mb-1">🔔 Segera Hadir</div>
                        <div class="text-xs text-gray-600 mb-3">Dapatkan notifikasi real-time</div>
                        <button class="w-full bg-primary-600 text-white text-xs font-medium px-3 py-2 rounded-md">
                            Daftar Waitlist
                        </button>
                    </div>
                </div>
            </div>
        </div>
        <!-- Gradient overlay at bottom to blend if needed, or just shadow -->
        <div class="absolute -inset-x-20 -bottom-20 h-40 bg-gradient-to-t from-white to-transparent pointer-events-none"></div>
    </div>
</section>

<style>
    @keyframes blob {
        0% { transform: translate(0px, 0px) scale(1); }
        33% { transform: translate(30px, -50px) scale(1.1); }
        66% { transform: translate(-20px, 20px) scale(0.9); }
        100% { transform: translate(0px, 0px) scale(1); }
    }
    .animate-blob {
        animation: blob 7s infinite;
    }
    .animation-delay-2000 {
        animation-delay: 2s;
    }
</style>
