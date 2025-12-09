<section class="py-24 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto">
    <h2 class="text-3xl sm:text-4xl font-bold text-center text-gray-900 mb-16 max-w-2xl mx-auto tracking-tight">
        Direct messages and quick<br />
        calls for everything in-between
    </h2>

    <div class="relative max-w-5xl mx-auto h-[400px]">
        <!-- Chat Interface (Background) -->
        <div class="absolute left-0 top-10 w-2/3 bg-white rounded-xl shadow-xl border border-gray-200 overflow-hidden flex h-80 z-10">
            <!-- Sidebar -->
            <div class="w-16 bg-gray-50 border-r border-gray-200 flex flex-col items-center py-4 gap-4">
                <img src="https://i.pravatar.cc/150?u=1" class="w-8 h-8 rounded-full" />
                <img src="https://i.pravatar.cc/150?u=2" class="w-8 h-8 rounded-full" />
                <div class="w-8 h-8 rounded-full bg-blue-500 flex items-center justify-center text-white text-xs">
                    <div class="w-2 h-2 bg-white rounded-full"></div>
                </div>
                <img src="https://i.pravatar.cc/150?u=3" class="w-8 h-8 rounded-full grayscale opacity-50" />
            </div>
            <!-- Chat Area -->
            <div class="flex-1 flex flex-col p-4 bg-white">
                <div class="flex-1 space-y-4">
                    <div class="flex gap-3">
                        <img src="https://i.pravatar.cc/150?u=2" class="w-8 h-8 rounded-full" />
                        <div class="space-y-1">
                            <div class="bg-gray-100 rounded-2xl rounded-tl-none px-4 py-2 text-sm text-gray-700 max-w-xs">
                                <div class="h-2 w-32 bg-gray-200 rounded-full mb-1"></div>
                                <div class="h-2 w-48 bg-gray-200 rounded-full"></div>
                            </div>
                        </div>
                    </div>
                    <div class="flex gap-3 flex-row-reverse">
                        <img src="https://i.pravatar.cc/150?u=me" class="w-8 h-8 rounded-full" />
                        <div class="space-y-1">
                            <div class="bg-blue-500 text-white rounded-2xl rounded-tr-none px-4 py-2 text-sm max-w-xs">
                                <div class="h-2 w-40 bg-white/30 rounded-full mb-1"></div>
                                <div class="h-2 w-24 bg-white/30 rounded-full"></div>
                            </div>
                             <div class="bg-blue-500 text-white rounded-2xl rounded-tr-none px-4 py-2 text-sm max-w-xs">
                                <div class="h-2 w-56 bg-white/30 rounded-full"></div>
                            </div>
                        </div>
                    </div>
                     <div class="flex gap-3">
                        <span class="text-2xl">👍</span>
                    </div>
                </div>
                <!-- Input -->
                <div class="mt-4 relative">
                    <div class="bg-gray-100 rounded-full h-10 w-full flex items-center px-4 gap-2">
                         <div class="w-6 h-6 rounded-full bg-green-500 flex items-center justify-center text-white text-xs">
                            <svg class="w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M23 7 16 12 23 17 23 7"/><rect x="1" y="5" width="15" height="14" rx="2" ry="2"/></svg>
                         </div>
                         <span class="text-sm font-medium text-gray-900">Started a call</span>
                         <div class="flex -space-x-1 ml-2">
                            <img src="https://i.pravatar.cc/150?u=1" class="w-5 h-5 rounded-full border border-white" />
                            <img src="https://i.pravatar.cc/150?u=2" class="w-5 h-5 rounded-full border border-white" />
                            <img src="https://i.pravatar.cc/150?u=3" class="w-5 h-5 rounded-full border border-white" />
                         </div>
                         <button class="ml-auto bg-green-600 text-white text-xs font-bold px-3 py-1 rounded-full">Join</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Video Call Grid (Foreground) -->
        <div class="absolute right-0 top-0 w-1/2 bg-gray-900 rounded-xl shadow-2xl border border-gray-800 overflow-hidden z-20 aspect-video">
            <div class="grid grid-cols-2 grid-rows-2 h-full">
                <div class="relative border-r border-b border-gray-800">
                    <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" class="w-full h-full object-cover opacity-80" />
                    <div class="absolute bottom-2 left-2 text-white text-xs font-medium">Sarah</div>
                </div>
                <div class="relative border-b border-gray-800">
                    <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" class="w-full h-full object-cover opacity-80" />
                    <div class="absolute bottom-2 left-2 text-white text-xs font-medium">Mike</div>
                </div>
                <div class="relative border-r border-gray-800">
                    <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" class="w-full h-full object-cover opacity-80" />
                    <div class="absolute bottom-2 left-2 text-white text-xs font-medium">Tom</div>
                </div>
                <div class="relative">
                    <img src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" class="w-full h-full object-cover opacity-80" />
                    <div class="absolute bottom-2 left-2 text-white text-xs font-medium">Emily</div>
                </div>
            </div>
            <!-- Controls -->
            <div class="absolute bottom-4 left-1/2 -translate-x-1/2 flex gap-2">
                 <button class="w-8 h-8 rounded-full bg-gray-800 flex items-center justify-center text-white hover:bg-gray-700">
                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>
                 </button>
                 <button class="w-8 h-8 rounded-full bg-gray-800 flex items-center justify-center text-white hover:bg-gray-700">
                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M23 7 16 12 23 17 23 7"/><rect x="1" y="5" width="15" height="14" rx="2" ry="2"/></svg>
                 </button>
                 <button class="w-8 h-8 rounded-full bg-red-600 flex items-center justify-center text-white hover:bg-red-700">
                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>
                 </button>
            </div>
        </div>
        
        <!-- Arrow connecting chat to video -->
         <div class="absolute bottom-0 left-1/2 translate-x-10 z-0">
             <svg width="60" height="40" viewBox="0 0 60 40" fill="none" class="text-gray-300 transform rotate-12">
                <path d="M10,30 Q30,40 50,10" stroke="currentColor" stroke-width="2" marker-end="url(#arrowhead-curved-2)" />
                <defs>
                    <marker id="arrowhead-curved-2" markerWidth="10" markerHeight="7" refX="10" refY="3.5" orient="auto">
                        <polygon points="0 0, 10 3.5, 0 7" fill="currentColor" />
                    </marker>
                </defs>
            </svg>
        </div>
    </div>
</section>
