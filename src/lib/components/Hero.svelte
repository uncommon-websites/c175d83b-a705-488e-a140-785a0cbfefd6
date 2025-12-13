<script lang="ts">
    import MockAppInterface from './MockAppInterface.svelte';
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

        <MockAppInterface />
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
