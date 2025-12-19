<script lang="ts">
    export let imageSrc: string;
    export let imageAlt: string;
    export let label: string;
    export let title: string;
    export let description: string;
    export let reversed: boolean = false;
    export let bgColor: string = "bg-[#F2F0EA]";
</script>

<section class="w-full flex flex-col md:flex-row {bgColor}">
    {#if reversed}
        <!-- Image Left, Text Right -->
        <div class="w-full md:w-1/2 h-[600px] md:h-[800px] relative">
            <img src={imageSrc} alt={imageAlt} class="w-full h-full object-cover" />
        </div>
        
        <div class="w-full md:w-1/2 flex flex-col items-center justify-center p-12 md:p-24 text-center">
             <span class="text-[10px] tracking-[0.2em] uppercase text-[#555] mb-8 font-sans">{label}</span>
             
             <h2 class="font-serif text-[32px] md:text-[36px] leading-[1.2] text-[#2A2A2A] max-w-lg mb-8 font-light">
                 {title}
             </h2>
             
             <p class="font-mono text-[13px] leading-[1.8] text-[#333] max-w-md mb-12 tracking-wide text-justify-center">
                 {description}
             </p>
             
             <a href="/" class="text-[10px] tracking-[0.2em] uppercase text-[#2A2A2A] border-b border-[#2A2A2A] pb-1 hover:opacity-70 transition-opacity font-sans">
                Explore More
            </a>
        </div>
    {:else}
        <!-- Text Left, Image Right -->
        <div class="w-full md:w-1/2 flex flex-col items-center justify-center p-12 md:p-24 text-center">
            <span class="text-[10px] tracking-[0.2em] uppercase text-[#555] mb-8 font-sans">{label}</span>
            
            <h2 class="font-serif text-[32px] md:text-[36px] leading-[1.2] text-[#2A2A2A] max-w-lg mb-8 font-light">
                {title}
            </h2>
            
            <p class="font-mono text-[13px] leading-[1.8] text-[#333] max-w-md mb-12 tracking-wide">
                {description}
            </p>
            
            <a href="/" class="text-[10px] tracking-[0.2em] uppercase text-[#2A2A2A] border-b border-[#2A2A2A] pb-1 hover:opacity-70 transition-opacity font-sans">
               Explore More
           </a>
       </div>

        <div class="w-full md:w-1/2 h-[600px] md:h-[800px] relative">
            <img src={imageSrc} alt={imageAlt} class="w-full h-full object-cover" />
        </div>
    {/if}
</section>
