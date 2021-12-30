<script>
	import {Router, Link, Route} from 'svelte-navigator'
	import Landing from './components/Landing.svelte'
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

	.main-body{
		margin-top: 10em;
		min-height: 75vh;
	}

	:global(a){
		text-decoration-color: rgb(255, 239, 208) 
	}
</style>


<Router>
	<Nav/>
	<div class="main-body">
	<Route path='/' component={Landing}/>
	<Route path='about' component={About}/>
	<Route path='coach' component={Coach}/>
	<Route path='clients' component={Clients}/>
	<Route path='pricing' component={Pricing}/>
	<Route path='contact' component={Contact}/>
	</div>
</Router>
<Footer/>

<!-- <Header/>
<About/>
<hr>
<Coach/>
<hr>
<Clients/>
<hr>
<Pricing/>
<hr>
<Contact/>
<Footer/> -->