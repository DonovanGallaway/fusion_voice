<script>
	import Header from './components/Header.svelte'
	import Nav from './components/Nav.svelte'
	import About from './components/About.svelte'
	import Coach from './components/Coach.svelte'
	import Clients from './components/Clients.svelte'
	import Pricing from './components/Pricing.svelte'
	import Contact from './components/Contact.svelte'
	import Footer from './components/Footer.svelte'
</script>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;400&display=swap');
	:global(html){
		scroll-behavior: smooth;
	}

	:global(*){
		font-family: 'Oswald', sans-serif;
	}

	:global(.section-title){
		color: rgb(255, 116, 0);
	}

	:global(p,li,h3, h5){
		color: rgb(155, 0, 0)
	}

	:global(button){
		border-radius: 10px;
		background-color: white;
		border: 2px solid black;
		color: black;
		text-align: right;
	}

	:global(button:hover){
		color:rgb(197, 0, 0);
		border: 2px solid rgb(197,0,0);
		cursor: pointer;
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
<Footer/>