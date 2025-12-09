<script lang="ts">
    export let pillText = "NEW";
    export let mainText = "Campsite is winding down";
    export let linkText = "Campsite's founders have joined Notion";
</script>

<div class="flex justify-center w-full py-12">
    <div class="inline-flex items-center gap-2 bg-orange-50 border border-orange-100 rounded-full px-1 py-1 pr-3 shadow-sm hover:bg-orange-100 transition-colors cursor-pointer group">
        <span class="bg-black text-white text-[10px] font-bold px-1.5 py-0.5 rounded-full tracking-wide">{pillText}</span>
        <span class="text-sm font-medium text-gray-900 flex items-center gap-1">
            {mainText}
            <svg viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4 text-gray-400"><path fill-rule="evenodd" d="M6.22 4.22a.75.75 0 0 1 1.06 0l3.25 3.25a.75.75 0 0 1 0 1.06l-3.25 3.25a.75.75 0 0 1-1.06-1.06L8.94 8 6.22 5.28a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" /></svg>
        </span>
        <span class="text-sm font-medium text-orange-600 flex items-center gap-1 group-hover:text-orange-700">
            {linkText}
            <div class="bg-orange-500 rounded-full p-0.5 text-white">
                <svg viewBox="0 0 16 16" fill="currentColor" class="w-3 h-3"><path fill-rule="evenodd" d="M6.22 4.22a.75.75 0 0 1 1.06 0l3.25 3.25a.75.75 0 0 1 0 1.06l-3.25 3.25a.75.75 0 0 1-1.06-1.06L8.94 8 6.22 5.28a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" /></svg>
            </div>
        </span>
    </div>
</div>
