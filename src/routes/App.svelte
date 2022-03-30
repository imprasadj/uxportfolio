<!-- <script>
	
import Heropage from "./Heropage.svelte";
import Projects from "./Projects.svelte";
import Versiondiv from '$lib/Footer.svelte';

</script>

<main id="bg">
  
    <div class="layout">
     
      <video id="background-video" autoplay loop muted poster="bgvideo.png">
        <source src="https://res.cloudinary.com/dgo4zxn5s/video/upload/v1647874441/bg-artwork/loopbg_u5hjk1.mp4" type="video/mp4">
      </video>
      <Heropage/>
	
    </div>
  <Projects/>
  <Versiondiv/>
  
</main>


<style>

.layout{
		
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0 20px;
  margin: 0 auto;

}  
 
#background-video {
  width: 100vw;
  height: 100vh;
  object-fit: cover;
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: -1;
}
#bg {
  background-position: center;
  background-repeat: repeat;
  background-attachment: fixed;
}



	/*===================================MEDIA-=====  */
  @media (min-width:700px){
    
    .layout{
      width: 87%;
      /* background-color: aqua; */
    } 
  }


</style> -->