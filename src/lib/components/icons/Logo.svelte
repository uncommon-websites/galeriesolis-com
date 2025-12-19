<script lang="ts">
    export let class_name = "";
</script>

<svg viewBox="0 0 100 200" class={class_name} fill="none" xmlns="http://www.w3.org/2000/svg">
    <!-- Outer Oval G shape -->
    <path d="M50 10 C 20 10, 10 40, 10 100 C 10 160, 20 190, 50 190 C 80 190, 90 160, 90 100 C 90 80, 85 60, 75 50" stroke="currentColor" stroke-width="1.5" />
    <path d="M50 190 C 40 190, 35 185, 35 175" stroke="currentColor" stroke-width="1.5" />
    
    <!-- Inner S shape intertwined -->
    <path d="M65 40 C 50 30, 30 40, 30 60 C 30 80, 70 90, 70 120 C 70 150, 40 160, 25 150" stroke="currentColor" stroke-width="1.5" />
    
    <!-- Decorative lines to mimic the complexity -->
    <path d="M50 15 C 80 15, 85 40, 85 100 C 85 160, 80 185, 50 185" stroke="currentColor" stroke-width="1" opacity="0.7"/>
    <path d="M50 15 C 20 15, 15 40, 15 100 C 15 160, 20 185, 50 185" stroke="currentColor" stroke-width="1" opacity="0.7"/>
    
    <!-- Vertical center line hint -->
    <path d="M50 20 L 50 180" stroke="currentColor" stroke-width="0.5" opacity="0.3" />
</svg>
