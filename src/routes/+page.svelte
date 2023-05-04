<script>
	import Testimonial from './Testimonial.svelte';
	import Hero from './Hero.svelte';
	import Banner from './Banner.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
  import Features from './Features.svelte';
  import Stats from './Stats.svelte';
  import Trusted from './Trusted.svelte';
  import About from './About.svelte';
</script>

<svelte:head>
	<title>The Future of Wealth: How to make money with ChatGPT</title>
<meta name="description" content="Discover the secrets to making money with ChatGPT! Our eBook, The Future of Wealth, reveals everything you need to know about this cutting-edge technology." />
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=AW-309362205"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'AW-309362205');
</script>
</svelte:head>

<section>
	<div class="flex-1 space-y-4">
	<Banner/>
	<Hero/>
	<About/>
	<Testimonial />
	<Trusted/>
	<Stats/>
</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

</style>
