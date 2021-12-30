<script>
    import {Router, Link, Route} from 'svelte-navigator'
</script>

<style>
    nav {
        position: fixed;
        width: 100%;
        top: 0;
        height: 5em;
    }
    .navbar {
        display: flex;
        justify-content: space-around;
        flex-direction: row;
        background-color: rgb(255, 75, 75);
        align-items: center;
    }

    h4, h1{
        color: rgb(255, 239, 208);
           
    }

    h1{
        font-size: 2em;
    }

    h4{
        font-size: 1.2em;
    }

    
</style>

<nav>
    <div class="navbar">
        <div class='logo'>
        <Link to='/'><h1>Fusion Voice Studios</h1></Link>
        <!-- <p>Make it happen.</p> -->
        </div>
            <Link to='about'><h4>What We Do</h4></Link>
            <Link to='coach'><h4>Coach</h4></Link>
            <Link to='clients'><h4>Clients</h4></Link>
            <Link to='pricing'><h4>Pricing</h4></Link>
            <Link to='contact'><h4>Contact</h4></Link>
            <!-- <a href="#testimonials"><h4>Testimonials</h4></a> -->
    </div>
</nav>