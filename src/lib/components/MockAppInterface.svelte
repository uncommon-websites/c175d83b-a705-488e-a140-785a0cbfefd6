<script lang="ts">
    // Mock data for the interface
    const favorites = [
        { name: "Ryan Nystrom", icon: "user" },
        { name: "Nick Holden", icon: "user" },
        { name: "Founders", icon: "lock" },
        { name: "Investor update Q3 ...", icon: "doc" }
    ];

    const channels = [
        { name: "Daily Updates", icon: "hash", color: "bg-orange-100 text-orange-600" },
        { name: "Investor updates", icon: "hash", color: "bg-yellow-100 text-yellow-600" },
        { name: "Product", icon: "hash", color: "bg-blue-100 text-blue-600" },
        { name: "Engineering", icon: "hash", color: "bg-purple-100 text-purple-600" },
        { name: "Feedback", icon: "hash", color: "bg-pink-100 text-pink-600" },
        { name: "GTM", icon: "hash", color: "bg-green-100 text-green-600" },
        { name: "noob", icon: "hash", color: "bg-gray-100 text-gray-600" },
        { name: "MRR", icon: "hash", color: "bg-indigo-100 text-indigo-600" },
        { name: "Calls", icon: "video", color: "bg-red-100 text-red-600" },
        { name: "Photostream", icon: "image", color: "bg-cyan-100 text-cyan-600" }
    ];

    const posts = [
        {
            title: "Customer feedback: Add support for auto-recording calls",
            author: "Ryan Nystrom",
            preview: "This is the fourth time this week, we should do this!",
            tag: "Plain",
            tagColor: "text-gray-500",
            icon: "P",
            iconBg: "bg-black"
        },
        {
            title: "Q4 initiatives",
            author: "Brian Lovin",
            preview: "Hey everyone, I wanted to share what we'll be tackling through the end of the ye...",
            tag: "Product",
            tagColor: "text-blue-500",
            icon: "📝",
            iconBg: "bg-gray-100"
        },
        {
            title: "Daily update - October 4, 2024",
            author: "Brian Lovin",
            preview: "Campbot: What did you work on today?",
            tag: "Daily updates",
            tagColor: "text-orange-500",
            icon: "📅",
            iconBg: "bg-white border"
        },
        {
            title: "Consolidating our Radix component system",
            author: "Ryan Nystrom",
            preview: "It's only a matter of time before we fork Radix",
            tag: "Engineering",
            tagColor: "text-purple-500",
            icon: "Rx",
            iconBg: "bg-white border"
        }
    ];

    const yesterdayPosts = [
        {
            title: "Meta ads experiment progress",
            author: "Nick Holden",
            preview: "Here's a quick update on our current ads results with three distinct profiles we're tr...",
            tag: "Q4 Growth",
            tagColor: "text-pink-500",
            icon: "M",
            iconBg: "bg-blue-600 text-white"
        },
        {
            title: "Frontier Forest upgraded to Pro with 8 seats (+$160 MRR)",
            author: "Dan Philibin",
            preview: "🙌 woo! Glad we finally got them over the finish line.",
            tag: "Stripe",
            tagColor: "text-indigo-500",
            icon: "S",
            iconBg: "bg-indigo-600 text-white"
        },
        {
            title: "Supporting reminders on chat threads",
            author: "Ryan Nystrom",
            preview: "One of the missing features for Campsite is to support reminders on ch...",
            tag: "Feedback",
            tagColor: "text-yellow-500",
            icon: "🔔",
            iconBg: "bg-yellow-100"
        }
    ];

    const team = [
        { name: "Brian Lovin", status: "Update status", online: true, img: "https://i.pravatar.cc/150?u=brian" },
        { name: "Dan Philibin", status: "Focus", online: true, img: "https://i.pravatar.cc/150?u=dan" },
        { name: "Alexandru Turcanu", online: true, img: "https://i.pravatar.cc/150?u=alex" },
        { name: "Nick Holden", online: true, img: "https://i.pravatar.cc/150?u=nick" },
        { name: "Ryan Nystrom", online: true, img: "https://i.pravatar.cc/150?u=ryan" },
        { name: "Paul Boudet", online: false, img: "https://i.pravatar.cc/150?u=paul" }
    ];
</script>

<div class="rounded-xl border border-gray-200 bg-white shadow-2xl overflow-hidden flex h-[800px] text-sm select-none relative z-10">
    <!-- Left Sidebar -->
    <div class="w-64 bg-gray-50 border-r border-gray-200 flex flex-col flex-shrink-0">
        <!-- Header -->
        <div class="p-3 border-b border-gray-200 flex items-center justify-between">
            <div class="flex items-center gap-2 font-medium text-gray-900">
                <div class="w-5 h-5 bg-orange-500 rounded flex items-center justify-center text-white text-xs font-bold">C</div>
                Acme, Inc.
                <svg class="w-3 h-3 text-gray-400" viewBox="0 0 16 16" fill="currentColor"><path d="M4 6l4 4 4-4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <div class="flex items-center gap-1">
                 <svg class="w-4 h-4 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M12 8v8M8 12h8"/></svg>
            </div>
        </div>

        <!-- New Post Button -->
        <div class="px-3 py-2">
            <button class="w-full bg-white border border-gray-200 rounded-md py-1.5 px-3 text-gray-600 font-medium text-left shadow-sm flex items-center gap-2 hover:bg-gray-50">
                <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
                New post
                <span class="ml-auto text-xs text-gray-400">C</span>
            </button>
        </div>

        <!-- Navigation -->
        <div class="flex-1 overflow-y-auto px-2 py-1 space-y-6">
            <!-- Main Links -->
            <div class="space-y-0.5">
                <div class="flex items-center gap-2 px-2 py-1 rounded-md bg-gray-200/50 text-gray-900 font-medium">
                    <svg class="w-4 h-4 text-gray-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
                    Home
                </div>
                <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                    <svg class="w-4 h-4 text-gray-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
                    Inbox
                </div>
                <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                    <svg class="w-4 h-4 text-gray-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
                    Messages
                </div>
                <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                    <svg class="w-4 h-4 text-gray-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
                    Docs
                </div>
                <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                    <svg class="w-4 h-4 text-gray-500" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
                    Calls
                </div>
            </div>

            <!-- Favorites -->
            <div>
                <div class="px-2 text-xs font-medium text-gray-400 mb-1">Favorites</div>
                <div class="space-y-0.5">
                    {#each favorites as fav}
                        <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                            {#if fav.icon === 'user'}
                                <div class="w-4 h-4 rounded-full bg-gray-300"></div>
                            {:else if fav.icon === 'lock'}
                                <svg class="w-3.5 h-3.5 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
                            {:else}
                                <svg class="w-3.5 h-3.5 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/></svg>
                            {/if}
                            <span class="truncate">{fav.name}</span>
                        </div>
                    {/each}
                </div>
            </div>

            <!-- Channels -->
            <div>
                <div class="px-2 text-xs font-medium text-gray-400 mb-1">Channels</div>
                <div class="space-y-0.5">
                    {#each channels as channel}
                        <div class="flex items-center gap-2 px-2 py-1 rounded-md text-gray-600 hover:bg-gray-100">
                            {#if channel.icon === 'hash'}
                                <span class="text-gray-400">#</span>
                            {:else if channel.icon === 'video'}
                                <svg class="w-3.5 h-3.5 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polygon points="23 7 16 12 23 17 23 7"/><rect x="1" y="5" width="15" height="14" rx="2" ry="2"/></svg>
                            {:else}
                                <svg class="w-3.5 h-3.5 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><circle cx="8.5" cy="8.5" r="1.5"/><polyline points="21 15 16 10 5 21"/></svg>
                            {/if}
                            <span class="truncate">{channel.name}</span>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>

    <!-- Main Content -->
    <div class="flex-1 flex flex-col bg-white min-w-0">
        <!-- Header -->
        <div class="px-8 py-6 pb-2">
            <h2 class="text-2xl font-bold text-gray-900 mb-4">Home</h2>
            <div class="flex items-center justify-between border-b border-gray-100 pb-0">
                <div class="flex gap-6">
                    <button class="pb-2 border-b-2 border-black font-medium text-gray-900">For me</button>
                    <button class="pb-2 border-b-2 border-transparent font-medium text-gray-500 hover:text-gray-700">Created</button>
                    <button class="pb-2 border-b-2 border-transparent font-medium text-gray-500 hover:text-gray-700">All</button>
                </div>
                <button class="text-gray-400 hover:text-gray-600 mb-2">
                    <svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="4" y1="21" x2="4" y2="14"/><line x1="4" y1="10" x2="4" y2="3"/><line x1="12" y1="21" x2="12" y2="12"/><line x1="12" y1="8" x2="12" y2="3"/><line x1="20" y1="21" x2="20" y2="16"/><line x1="20" y1="12" x2="20" y2="3"/><line x1="1" y1="14" x2="7" y2="14"/><line x1="9" y1="8" x2="15" y2="8"/><line x1="17" y1="16" x2="23" y2="16"/></svg>
                </button>
            </div>
        </div>

        <!-- Input -->
        <div class="px-8 py-4">
            <div class="flex gap-3 items-start">
                <div class="w-8 h-8 rounded-full bg-gray-200 flex-shrink-0"></div>
                <div class="flex-1 relative">
                    <input type="text" placeholder="What do you want to share?" class="w-full bg-transparent text-gray-900 placeholder-gray-400 focus:outline-none py-1.5" />
                </div>
                <button class="px-3 py-1.5 bg-gray-100 text-gray-400 rounded-md text-xs font-medium">Post</button>
            </div>
        </div>

        <!-- Feed -->
        <div class="flex-1 overflow-y-auto px-8 pb-8">
            <!-- Today -->
            <div class="mb-6">
                <h3 class="text-xs font-medium text-gray-400 mb-3">Today</h3>
                <div class="space-y-4">
                    {#each posts as post}
                        <div class="group flex gap-3 items-start">
                            <div class="w-8 h-8 rounded-md {post.iconBg} flex items-center justify-center text-white text-xs font-bold flex-shrink-0 mt-0.5 shadow-sm border border-black/5">
                                {#if post.icon === 'P'}
                                    <span class="font-serif italic">P</span>
                                {:else}
                                    {post.icon}
                                {/if}
                            </div>
                            <div class="flex-1 min-w-0">
                                <div class="flex items-baseline gap-2">
                                    <span class="font-medium text-gray-900 truncate">{post.title}</span>
                                </div>
                                <div class="flex items-center gap-1.5 text-gray-500 text-xs mt-0.5">
                                    <span class="font-medium text-gray-600">{post.author}:</span>
                                    <span class="truncate">{post.preview}</span>
                                </div>
                            </div>
                            <div class="flex items-center gap-2 flex-shrink-0">
                                <span class="text-[10px] font-medium px-1.5 py-0.5 rounded bg-gray-50 {post.tagColor} border border-gray-100">{post.tag}</span>
                            </div>
                        </div>
                    {/each}
                </div>
            </div>

            <!-- Yesterday -->
            <div>
                <h3 class="text-xs font-medium text-gray-400 mb-3">Yesterday</h3>
                <div class="space-y-4">
                    {#each yesterdayPosts as post}
                        <div class="group flex gap-3 items-start">
                             <div class="w-8 h-8 rounded-md {post.iconBg} flex items-center justify-center text-white text-xs font-bold flex-shrink-0 mt-0.5 shadow-sm border border-black/5">
                                {post.icon}
                            </div>
                            <div class="flex-1 min-w-0">
                                <div class="flex items-baseline gap-2">
                                    <span class="font-medium text-gray-900 truncate">{post.title}</span>
                                </div>
                                <div class="flex items-center gap-1.5 text-gray-500 text-xs mt-0.5">
                                    <span class="font-medium text-gray-600">{post.author}:</span>
                                    <span class="truncate">{post.preview}</span>
                                </div>
                            </div>
                            <div class="flex items-center gap-2 flex-shrink-0">
                                <span class="text-[10px] font-medium px-1.5 py-0.5 rounded bg-gray-50 {post.tagColor} border border-gray-100">{post.tag}</span>
                            </div>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>

    <!-- Right Sidebar -->
    <div class="w-64 border-l border-gray-200 bg-gray-50 flex flex-col flex-shrink-0">
        <div class="p-3">
             <div class="relative">
                <svg class="absolute left-2.5 top-2 w-4 h-4 text-gray-400" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><line x1="21" y1="21" x2="16.65" y2="16.65"/></svg>
                <input type="text" placeholder="Search people..." class="w-full bg-white border border-gray-200 rounded-md pl-9 pr-3 py-1.5 text-sm placeholder-gray-400 focus:outline-none focus:border-gray-300" />
            </div>
        </div>

        <div class="flex-1 overflow-y-auto px-3 py-2">
            <div class="flex items-center gap-1.5 text-xs text-gray-400 font-medium mb-3">
                <div class="w-1.5 h-1.5 rounded-full bg-green-500"></div>
                4 online
            </div>
            
            <div class="space-y-3">
                {#each team as member}
                    <div class="flex items-start gap-2">
                        <div class="relative">
                            <img src={member.img} alt={member.name} class="w-8 h-8 rounded-full bg-gray-200" />
                            {#if member.online}
                                <div class="absolute -bottom-0.5 -right-0.5 w-2.5 h-2.5 bg-green-500 border-2 border-gray-50 rounded-full"></div>
                            {/if}
                        </div>
                        <div class="flex-1 min-w-0">
                            <div class="text-sm font-medium text-gray-900 truncate">{member.name}</div>
                            {#if member.status}
                                <div class="text-xs text-gray-500 truncate flex items-center gap-1">
                                    {#if member.status === 'Focus'}
                                        <span>🧘</span>
                                    {/if}
                                    {member.status}
                                </div>
                            {/if}
                        </div>
                    </div>
                {/each}
            </div>

             <div class="mt-6">
                <div class="flex items-center gap-1.5 text-xs text-gray-400 font-medium mb-3">
                    <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
                    Guests
                </div>
            </div>
        </div>
    </div>
</div>
