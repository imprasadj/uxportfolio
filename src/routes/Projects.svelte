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
    PROJECTS
</h2>
</div>
<section class="projects" id="projects">
    
    <div class="container3">
        <div class="textcontainer">
            <div class="text" data-aos="fade-in" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>01</p>
                <h1>Pune Metro</h1>
                <h3>Rebranding and redesign of city's first ever Metro rail</h3>
                <h4>
                    <a href="https://www.behance.net/gallery/144895185/Pune-Metro-Rebranding-Redesign" target="_blank">
                        <button>Go to project</button></a>
                </h4>
            </div>
        </div>
    </div>
    
    <div class="container2">
        <div class="textcontainer">
            <div class="text" data-aos="fade-in" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>02</p>
                <h1>NayeNayan</h1>
                <h3>Landing page design for Bhumi NGO</h3>
                <h4>
                    <a href="https://www.behance.net/gallery/144681549/App-development-Agency%28fictional%29" target="_blank">
                       <button>Go to project</button></a>
                </h4>    
            </div>
        </div>
    </div>

    <div class="container4">
        <div class="textcontainer">
            <div class="text" data-aos="fade-in" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>03</p>
                <h1>RESQ</h1>
                <h3>Webapp redesign for the only rescue unit in the city</h3>
                <h4>
                    <a href="https://www.behance.net/gallery/124483607/Animal-Rescue-Webapp-redesign" target="_blank" >
                        <button>Go to project</button></a>
                </h4>       
            </div>
        </div>
    </div>
    
    <div class="container1">
        <div class="textcontainer">
            <div class="text" data-aos="fade-in" data-aos-duration="500" data-aos-anchor-placement="bottom-bottom">
                <p>04</p>
                <h1>HMI</h1>
                <h3>A dashboard display concept(wip)</h3>
                <h4>
                    <a href="https://www.behance.net/gallery/142381103/Vehicle-HMI-Display-%28concept%29" target="_blank" >
                        <button>Go to project</button></a>
                </h4>       
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
    background-color: rgba(0, 0, 0, 0.696);    
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
    font-family: var(--bodyfont);
}
h3{
    margin: 2rem 0 0 0;
    font-weight: 300;
    font-size: 1.1rem;
}
h4{
    margin-top: 1.5rem;
    font-weight: 300;
}
button{
    font-family: var(--bodyfont);
    padding: 1rem;
    background-color: rgb(255, 255, 255);
    border-radius: .1rem;
    border-style: none;
    transition: .2s ease-in-out;
    cursor: pointer;
}
button:hover{
    letter-spacing: .5px;
}

a{  
    text-decoration: none;
    transition: .2s ease-out;
    color: rgb(0, 0, 0);
    /* border-bottom:1px solid rgb(165, 165, 165); */
}


.text{
    /* padding: .5rem; */
    margin-left:8%;
    margin-right: 6%;
    padding-top: 10rem;
    color: rgb(255, 255, 255) !important;
}

.container1{
    z-index: 50;
    width: 100%;
    top: 100vh;
    height: 100vh;
    background-color: rgb(243, 243, 243);
    background-image: url("/hmi.png");
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
    background-image: url("/Nayenayan.webp");
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
    background-image: url("/Metro.webp");
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
}

.container4{
    z-index: 50;
    width: 100%;
    top: 100vh;
    height: 100vh;
    background-color: rgb(243, 243, 243);
    background-image: url("/resq3.png");
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
}

/* ==============Media Queries============================ */

@media (min-width:800px){
.textcontainer{
    width: 50%;
    background-color: rgba(0, 0, 0, 0.475);
    backdrop-filter: blur(2px);
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