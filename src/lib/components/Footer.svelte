<script lang="ts">
    import Logo from "$lib/components/icons/Logo.svelte";
</script>

<footer class="w-full bg-[#F2F0EA] pt-24 pb-8 px-6 md:px-12 border-t border-[#E5E2D9]">
    <div class="flex flex-col md:flex-row justify-between items-start mb-24">
        <!-- Newsletter -->
        <div class="w-full md:w-1/3 mb-12 md:mb-0">
            <h3 class="font-serif text-2xl text-[#2A2A2A] mb-6 font-light">Join our List</h3>
            <p class="font-mono text-[11px] text-[#555] mb-8 max-w-xs leading-relaxed">
                Sign up for our newsletter to receive the latest launches and news
            </p>
            
            <form class="w-full max-w-xs relative border-b border-[#999] pb-2">
                <input type="email" class="w-full bg-transparent border-none outline-none text-sm font-mono placeholder:text-transparent" />
                <button type="submit" class="absolute right-0 bottom-2 text-[#555] hover:text-black">
                    <svg width="20" height="10" viewBox="0 0 20 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M15 1L19 5L15 9" stroke="currentColor" stroke-width="0.7"/>
                        <path d="M0 5H19" stroke="currentColor" stroke-width="0.7"/>
                    </svg>
                </button>
            </form>
        </div>

        <!-- Links -->
        <div class="w-full md:w-1/3 flex justify-end gap-16 md:gap-24 text-[10px] tracking-[0.1em] uppercase font-sans text-[#333]">
            <div class="flex flex-col gap-4">
                <a href="/" class="hover:opacity-60 transition-opacity">Our Story</a>
                <a href="/" class="hover:opacity-60 transition-opacity">Contact</a>
                <a href="/" class="hover:opacity-60 transition-opacity">Design Studio</a>
            </div>
            <div class="flex flex-col gap-4">
                <a href="/" class="hover:opacity-60 transition-opacity">Shipping +<br>Returns</a>
                <a href="/" class="hover:opacity-60 transition-opacity">Privacy</a>
                <a href="/" class="hover:opacity-60 transition-opacity">Terms</a>
            </div>
        </div>
    </div>

    <!-- Bottom Logo & Copyright -->
    <div class="flex flex-col items-center justify-center relative">
        <div class="mb-4">
            <Logo class_name="h-32 w-16 text-[#3C2D25]" />
        </div>
        <div class="text-center mb-8">
            <h2 class="font-serif text-sm tracking-widest font-bold text-[#3C2D25] uppercase">Galerie Solis</h2>
            <span class="text-[8px] tracking-[0.1em] text-[#3C2D25] uppercase mt-1 block">Est. 2023</span>
        </div>
        
        <div class="w-full flex justify-between items-end text-[9px] uppercase tracking-[0.05em] text-[#555] font-sans absolute bottom-0 w-full">
            <span>© Galerie Solis 2024 All Rights Reserved</span>
            <a href="/" class="underline decoration-1 underline-offset-2">Site Credits</a>
        </div>
    </div>
    
    <!-- Mobile fix for absolute positioning of copyright -->
    <div class="md:hidden flex flex-col items-center gap-4 mt-8 text-[9px] uppercase tracking-[0.05em] text-[#555] font-sans">
        <span>© Galerie Solis 2024 All Rights Reserved</span>
        <a href="/" class="underline decoration-1 underline-offset-2">Site Credits</a>
    </div>
</footer>
