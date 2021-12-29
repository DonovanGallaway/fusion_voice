<script>
    const prices = [
        {name: "KIDS LESSONS (Piano, Guitar or Voice", notes: "In person or on video", time: "30 min", price: "$45"},
        {name: "ADULT GUITAR OR PIANO LESSONS", notes: "In person or on video", time: "45 min", price: "$60"},
        {name: "ADULT VOICE LESSONS", notes: "In person or on video", time: "45 min", price: "$60"},
        {name: "BLOCK LESSON DISCOUNTS", notes: "Discounts on block lessons and when you enroll in two or more services", time: "45 min", price: "From $450-$600"},
        {name: "SONG RECORDING AND MUSIC PACKAGE", notes: "Reduced price for kids!", time: "8 hrs", price: "$1500"},
        {name: "90-DAY COACHING PROGRAM", notes: "For professional artists pursuing a music career. In person or on video", time: "30 hrs", price: "$1500"}
    ]
</script>

<style>
    .price-wrapper{
        width: 50%;
        margin: auto;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .price-wrapper > *{
        margin: 2em;
    }

    .price-numbers {
        text-align: right;
    }

    h2{
        text-align: center;
    }
</style>

<div id="pricing">
    <h2 class="section-title">PRICING</h2>
    <div class="pricing-wrapper">
        {#each prices as price}
            <div class="price-wrapper">
                <div class="price-description">
                    <h3>{price.name}</h3>
                    <p>{price.notes}</p>
                </div>
                <div class="price-numbers">
                    <h5>{price.time}</h5>
                    <h5>{price.price}</h5>
                </div>
            </div>
        {/each}
    </div>
</div>