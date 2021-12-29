<style>
    *{
        text-align: center;
    }

    #contact{
        width: 30vw;
        margin: auto;
    }

    form {
        padding: 3em;
        border: 2px double black;
    }

    .contact-wrapper{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }

    .contact-wrapper > *{
        margin: 3em;
    }
</style>

<div id="contact">
    <h2>Contact Us</h2>
    <div class="contact-wrapper">
        <div class="contact-img-wrapper">
            <img alt="fusion voice logo" src="/banner.png"/>
        </div>
        <div class="form-wrapper">
            <form>
                <label for='name'>Name: <br>
                <input type="text" name="name"/>
                </label>
                <label for='email'>Email: <br>
                <input type="text" name="email"/>
                </label>
                <label for="phone">Phone: <br>
                <input type="text" name="phone"/>
                <label for="message">Message (Optional): <br>
                <input type="textarea" name='message'/>
                </label>
            </form>
        </div>
    </div>
    
    <div class="social-bar">
        <a href="https://www.facebook.com/FusionVoiceStudios/"><img alt="facebook link" src="https://img.icons8.com/color/48/000000/facebook-new.png"/></a>
        <a href="https://twitter.com/Fusion_Voice"><img alt="twitter link" src="https://img.icons8.com/fluency/48/000000/twitter.png"/></a>
        <a href="https://www.youtube.com/channel/UCkAiypWjrplb3CkWogyT2jQ"><img alt="youtube link" src="https://img.icons8.com/color/48/000000/youtube-play.png"/></a>
        <a href="https://www.instagram.com/fusionvoicestudios/"><img alt="instagram link" src="https://img.icons8.com/color/48/000000/instagram-new--v1.png"/></a>
    </div>
</div>