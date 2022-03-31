<script>
import { onMount } from 'svelte';
onMount(() => {
		
    var bgscroll = document.getElementById('background-video')
    window.addEventListener('scroll',()=>{
      bgscroll.style.opacity = 1 - +window.pageYOffset/380+''
      bgscroll.style.top =  +window.pageYOffset+'px'
      bgscroll.style.backgroundPositionY = - +window.pageYOffset/2+'px'  
    })
    
    var herotext = document.getElementById('hero')
    window.addEventListener('scroll',()=>{
      herotext.style.opacity = 1 - +window.pageYOffset/300+''
      herotext.style.top =  +window.pageYOffset+'px'   
    })

  });

</script>

<div id="hero-page">
    <video id="background-video" autoplay loop muted poster="bgvideo.png">
        <source src="https://res.cloudinary.com/dgo4zxn5s/video/upload/v1647874441/bg-artwork/loopbg_u5hjk1.mp4" type="video/mp4">
      </video>
    <section class="hero" id="hero">
        <div class="hero-text" id="hero-text"> 
            <h1 class="gradient" data-aos="fade-in" data-aos-duration="2000" data-aos-delay="500" data-aos-anchor-placement="bottom">
            WELCOME
            </h1>
                <p data-aos="fade-in" data-aos-duration="2000" data-aos-delay="1000" data-aos-anchor-placement="bottom">
                I am Prasad, <br>I'm a Experience Designer. 
                </p>
        </div>
        <div class="arrow-container" data-aos="fade-in" data-aos-duration="2000" data-aos-delay="2000" data-aos-anchor-placement="bottom">
            <div class="arrow-down"></div>
        </div>
    </section>
    
</div>

<style>

#hero-page{
    width:100%;
    z-index: 4;
}
#background-video {
      width: 100%;
      height: 100vh;
      object-fit: cover;
      position: absolute;
      left: 0;
      right: 0;
      top: 0;
      bottom: 0;
      z-index: -1;
    }
.hero{
    width: 100%;
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    align-items: left;
   
}


h1{ 
    font-weight: 700;
    letter-spacing: 1rem;
    font-size: 2.2rem;
    line-height: 83%;
    text-align: center;
    z-index: 5;
    
    background: linear-gradient(-70deg, #ffdf86e0, #ffffff6c, #ffffffe1,#c59ae9be,#ffffff88);
    background-size: auto;
    background-clip: border-box;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-size: 400% 400%;
    animation: gradient 11s ease infinite;
}
@keyframes gradient{
    0% {
  background-position: 0% 50%;
}
50% {
  background-position: 100% 10%;
}
100% {
  background-position: 0% 50%;
}
}

p{  
    font-size: 1.3rem;
    text-align: center;
    margin: 0;
    line-height: 170%;
    color: var(--maintext);
}


.arrow-container {
    align-self: center;
    margin: 5rem 0 0 0;
    width: 10px;
    /* cubic-bezier-easing = sine / mehr Beispiele: https://easings.net/ */
    animation: bounce 1600ms infinite cubic-bezier(0.445, 0.05, 0.55, 0.95);
    cursor: pointer;
    height: 30px;
}

.arrow-down {
  height: 1.2px;
  background: rgb(255, 255, 255);
  transform: rotate(45deg);
  transform-origin: 0% 0%;
  border-radius: 5px;
}
.arrow-down:after {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  bottom: 0;
  left: 100%;
  border-radius: 5px;
  background: rgb(255, 255, 255);
  transform: rotate(-90deg);
  transform-origin: 0% 100%;
}

@keyframes bounce {
50% {
    transform: translateY(-15px);
  }
}




/* ----------------------------MEDIA QUERIES----------------------- */

@media (min-width:800px){
    h1{
        font-size: 4rem;
        
    }
    .hero-text{
        text-align: left;
    }
    .gradient{
        background-size:80% auto;
    }
    

}
</style>