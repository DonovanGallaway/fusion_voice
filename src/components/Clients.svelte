<script>
    const clients = [
        {name: "Stewart Taylor", 
        description: "Stewart Taylor is a 24 year-old Pop/R&B singer, songwriter and dancer. A Berklee College of Music graduate, Stewart has worked with Grammy-nominated songwriters Kara DioGuardi (P!nk, Katy Perry), Charlie Puth (Wiz Khalifa) and The 3leven (Meagan Trainor).",
        link: "https://www.youtube.com/watch?v=l6oRgUAo4R8",
        img: "/stewart_taylor.jpg"
        },
        {name: "Jack Wesley",
        description: "22 year old Singer/Songwriter from Boston, MA. Influences include Zac Brown Band, Andy Grammer, Rob Thomas, Huey Lewis, Justin Timberlake, and more!",
        link: "https://www.youtube.com/watch?v=-PV2aOqmqAQ",
        img: "/jack_wesley.jpg"},
        {name: "Patrice Peris",
        description: "With soaring vocals and boundless energy, Patrice Peris is a cut above the rest. A self-described “mess of glamour with some funk and edge,” this R&B songstress is poised to crash the charts. She’s got the power of Christina Aguilera, the grittiness of Fergie and Rihanna, and the lyrical command of Alicia Keys.",
        link: "https://www.youtube.com/watch?v=jm14Tcv8_Vs",
        img: "patrice_peris.jpg"}
    ]
</script>

<style>
    h2{
        text-align: center;
    }
    .client-wrapper{
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 80%;
        margin: auto;
    }

    .client-text{
        width: 25%;
    }

    .client-img > img{
        object-fit: cover;
        border-radius: 50%;
        width: 200px;
        height: 200px;
    }

    @media screen and (max-width: 768px){
        .client-wrapper{
            flex-direction: column;
        }
    }
</style>

<div id="clients">
    <h2>Clients</h2>
    {#each clients as client}
        <div class="client-wrapper">
            <div class="client-img">
                <img src={client.img} alt={client.name}/>
            </div>
            <div class="client-text">
                <h4>{client.name}</h4>
                <p>{client.description}</p>
                <a href={client.link}><button>Watch Their Video</button></a>
            </div>
        </div>
    {/each}
</div>