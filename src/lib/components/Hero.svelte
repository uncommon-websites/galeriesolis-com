<script lang="ts">
    import Logo from "$lib/components/icons/Logo.svelte";
</script>

<section class="relative w-full h-screen bg-black flex items-center justify-center overflow-hidden">
    <!-- Logo Background -->
    <div class="relative z-10 flex flex-col items-center justify-center opacity-60 scale-110">
        <Logo class_name="h-80 w-40 text-[#8C6A5A]" />
    </div>

    <!-- Error Message Overlay (from screenshot) -->
    <div class="absolute z-20 flex flex-col items-center justify-center text-center w-full px-4">
        <h1 class="text-white font-sans text-2xl md:text-3xl font-bold mb-2 tracking-tight">
            We couldn't verify the security of your connection.
        </h1>
        <p class="text-gray-300 font-sans text-xs md:text-sm max-w-xl">
            Access to this content has been restricted. Contact your internet service provider for help.
        </p>
    </div>
</section>
