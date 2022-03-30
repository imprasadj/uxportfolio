<script>
	import '../global.css';
    import Heropage from "./Heropage.svelte";
    import Projects from "./Projects.svelte";
        
    </script>
    <svelte:head>
      <link rel="stylesheet" href="https://unpkg.com/aos@2.3.1/dist/aos.js">
    </svelte:head>


    <main id="bg">
      
        <div class="layout">
         
          
          <Heropage/>
        
        </div>
      <Projects/>
           
    </main>
    
    
    <style>
    
    .layout{
         
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0 20px;
      margin: 0 auto;
    
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
    
    
    </style>