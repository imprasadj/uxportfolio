<script>
    import { onMount } from 'svelte';
    onMount(() => {
		
    var bgscroll = document.getElementById('projects')
    window.addEventListener('scroll',()=>{
      bgscroll.style.opacity = -2 +window.pageYOffset/250+''
      bgscroll.style.top =  +window.pageYOffset+'px' 
      
    })
    
    
    });
</script>
<div class="proj" id="proj">
<h2 data-aos="zoom-in">
    Projects
</h2>
</div>
<section class="projects" id="projects">
    
    
    <div class="container2">
        <div class="textcontainer">
            <div class="text" data-aos="fade-up" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>01</p>
                <h1>Tesla</h1>
                <h3>Display UI for right hand driving systems</h3>
                <a href="/teslaux">Go to project</a>
            </div>
        </div>
    </div>
    <div class="container3">
        <div class="textcontainer">
            <div class="text" data-aos="fade-up" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>02</p>
                <h1>RESQ</h1>
                <h3>App redesign for city's only animal rescue unit</h3>
                <a href="/resqux">Go to project</a>
            </div>
        </div>
    </div>
    <div class="container1">
        <div class="textcontainer">
            <div class="text" data-aos="fade-up" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>03</p>
                <h1>AC controls</h1>
                <h3>Interaction on a vertical display concept(wip)</h3>
                <a href="/hmiux">Go to project</a>
            </div>
        </div>
    </div>

</section>

<!-- ===========================STYLES===================================== -->
<style>

.projects{
    align-items: center;
    margin: 0;
    width:100%;
    display: flex;
    flex-direction: column;
    z-index: 10;
    opacity: 0;
}
h2{
    text-transform: capitalize;
    font-size: 1.8rem;
    font-weight: 500;
    text-align: center;
    padding: 4rem 0 4rem 0;
    color: var(--maintext);
}

.textcontainer{
    position: absolute;
    right:0;
    height: 100vh;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.644);    
    backdrop-filter: blur(2px);
    -webkit-backdrop-filter: blur(2px);
}
p{
    font-size: 2.3rem;
    margin: .1rem 0;
    font-weight: 200;
}
h1{
    margin: 0;
    font-weight: 500;
    font-size: 3rem;
}
h3{
    margin: 2rem 0 .8rem 0;
    font-weight: 300;
    font-size: 1.1rem;
}
.text a{
    text-decoration: none;
    padding-top:1rem;
    border-bottom: 2px solid white;
    transition: .2s ease-out;
}
.text a:hover{
    letter-spacing: 1px;
}

.text{
    padding: .5rem;
    margin-left:10%;
    margin-right: 4%;
    padding-top: 10rem;
    color: aliceblue !important;
}

.container1{
    z-index: 50;
    width: 100%;
    top: 100vh;
    height: 100vh;
    background-color: rgb(243, 243, 243);
    background-image: url("/musicui.webp");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
}
.container2{
    z-index: 50;
    width: 100%;
    top: 100vh;
    height: 100vh;
    background-color: rgb(243, 243, 243);
    background-image: url("/Teslamockup.webp");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    
}

.container3{
    z-index: 50;
    width: 100%;
    top: 100vh;
    height: 100vh;
    background-color: rgb(243, 243, 243);
    background-image: url("/resq3.webp");
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
}



/* ==============Media Queries============================ */

@media (min-width:800px){
.textcontainer{
    width: 50%;
    backdrop-filter: blur(5px);
    -webkit-backdrop-filter: blur(5px);
}
h2{
    font-size: 2rem;
    font-weight: 700;
}
h3{
    font-size: 1.3rem;
}
}

</style>