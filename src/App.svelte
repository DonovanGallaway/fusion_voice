<script>
	import Header from './components/Header.svelte'
	import Nav from './components/Nav.svelte'
	import About from './components/About.svelte'
	import Coach from './components/Coach.svelte'
	import Clients from './components/Clients.svelte'
	import Pricing from './components/Pricing.svelte'
	import Contact from './components/Contact.svelte'
</script>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;400&display=swap');
	:global(html){
		scroll-behavior: smooth;
	}

	:global(*){
		font-family: 'Oswald', sans-serif;
	}


	
</style>

<Nav/>
<Header/>
<About/>
<hr>
<Coach/>
<hr>
<Clients/>
<hr>
<Pricing/>
<hr>
<Contact/>