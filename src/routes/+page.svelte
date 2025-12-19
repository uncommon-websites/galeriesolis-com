<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import Hero from "$lib/components/Hero.svelte";
	import SectionIntro from "$lib/components/SectionIntro.svelte";
	import SectionSplit from "$lib/components/SectionSplit.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<div class="bg-[#F2F0EA] min-h-screen text-[#1A1A1A] font-serif selection:bg-[#A67C6D] selection:text-white">
	<Header />
	
	<main>
		<Hero />
		
		<SectionIntro />
		
		<SectionSplit 
			imageSrc="https://images.unsplash.com/photo-1528458909336-e7a0adfed0a5?q=80&w=1200&auto=format&fit=crop" 
			imageAlt="Linen fabric"
			label="FABRIC"
			title="Belgian Stonewashed Linen, Italian Velvet and Mohair"
			description="Galerie Solis's textiles are produced in the oldest mills in Europe by masters of their craft. The linen is sourced from Belgium, and has been made sustainably over centuries, dyed in the tones that Sarah Solis has perfected. Similarly, the luxury mohairs and velvets come from a century-old mill in Italy that has historically created fabrications for the royal family and the Vatican."
			reversed={true}
			bgColor="bg-[#D6D2C9]" 
		/>

		<SectionSplit 
			imageSrc="https://images.unsplash.com/photo-1565538810643-b5bdb714032a?q=80&w=1200&auto=format&fit=crop" 
			imageAlt="Interior room with staircase"
			label="ANTIQUES"
			title="Furniture, Rugs, and Lighting"
			description="The third pillar of Galerie Solis is a curation of art and specialized estate and vintage objects hand-chosen by Sarah. She selects items that have stories that evolve over time. Those who live with pieces with well-earned patina continue to affect them, leaving their own indelible imprints. Sarah believes that imperfections are what create the extraordinary."
			reversed={false}
		/>
	</main>

	<Footer />
</div>

