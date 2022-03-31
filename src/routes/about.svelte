<script>
import Navbar from "$lib/Navbar.svelte";

</script>
<div class="aboutpage">
    <div class="title">
        <h1>ABOUT.</h1>
    </div>

    <div class="aboutbox">
            <div class="overlay">
                <div class="left">
                    <h2>Hello,<br/> <p>I'm a UX Designer who believes in thoughtfully crafted design.
                        Experience design helps me to have my technical knowledge 
                        and my creativity all at the same place to create design solutions.
                        </p>
                    </h2>
                </div>
            </div>
               
            
    </div>

    <div class="resume" id="resume">
        <h3>Resumé</h3>
        <div class="resumebox">
            <img src="/resume.webp" alt="">
        </div>
        <a href="https://drive.google.com/uc?export=download&id=1ajAUptgS05EmKmivKASB5QNnKypciU-c">
            <button>Download Resume</button>
        </a>
        
    </div>
    
</div>




<style>

    .aboutpage{
    margin: 0;
    width:100%;
    display: flex;
    flex-direction: column;
    z-index: 10;
           
    }
    .title{
        padding: 5% 7%;
        margin: 1rem 0;      
        text-align: center;
        color: rgb(255, 255, 255);
        
    }
    h1{
        font-size: 3rem;
        background: linear-gradient(-35deg, #fcfcfc91, #ffffff, #ffffff11,#eeeeeefb,#ffffff7c);
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
        background-position: 88% 50%;
        }
        100% {
        background-position: 0% 50%;
        }
    }
    h2{
        font-size: 2rem;
        font-weight: 600;
        color: var(--maintext);
        margin: 6rem 7rem;  
        line-height: 2.3rem;
        align-items: center;
        justify-content: center;  
    }

    .aboutbox{
    z-index: 7;
    width: 100%;
    height: 35rem;
    background-color: rgb(243, 243, 243);
    background-image: url("/photo.webp");
    background-size: 100%;
    
    background-position:center;
    background-attachment:scroll;
    }
    
    .overlay{
    position: absolute;
    left:0;
    height: 35rem;
    width: 50%;
    background-color: rgba(0, 0, 0, 0.74);    
    backdrop-filter: blur(2px);
    -webkit-backdrop-filter: blur(2px);
    }

    .resume{
        text-align: center;
        margin: 3rem 0;
        padding: 0 7%;
    }
    h3{
        font-size: 1.8rem;
        color: var(--maintext);
         
    }
    .resumebox{
        margin-bottom: 2rem;
    }
    img{
        width: 500px;
        height: auto;
        box-shadow: 1px 10px 25px #000000;
    }
    button{
        padding: 1.1rem 3rem;
        font-size: 1.1rem;
        border: none;
        transition: 0.3s;
    }
    button:hover{
        cursor: pointer;
        background-color: rgb(102, 194, 255);
    }
/* ---------------------------------------------------MEDIA QUERIES */
    @media (max-width:815px){
        img{
            width: 300px;
        }

        .overlay{
            width: 100%;
        }
        h2{ 
            font-size: 1.3rem;
            margin: 10% 2.2rem;
        }
        .aboutbox{
            background-size: auto;
            background-position: right;
        }

    }


</style>