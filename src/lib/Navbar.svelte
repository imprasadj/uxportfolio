<script>
import { Icon, MenuAlt4,X } from "svelte-hero-icons";


function openNav() {
    document.getElementById("mobile-menu").style.width="100%";
}
function closeNav() {
    document.getElementById("mobile-menu").style.width="0";
    document.getElementById("linktap").style.width="0";
}
</script>



<header>
   
    <a class="logo" href="/">prsΔd</a>
    <nav>
        <ul class="nav-links">
            <li><a href="/">home</a></li>
            <li><a href="/#proj">work</a></li>
            <li id="linktap"><a href="/about">about</a></li>
        </ul>
    </nav>
    <a class="resume" href="/about#resume">RESUMÉ</a>
    <div class="menu" on:click={() => openNav()} >
        <Icon src="{MenuAlt4}" size="24" color="white" solid/>
    </div>
</header>

<div id="mobile-menu" class="overlay">
    <div class="close" on:click={() => closeNav()}>
        <Icon src="{X}" size="24" color="white" solid/>
    </div>
    <div class="overlay-content" on:click={() => closeNav()}>
        <li><a href="/">home</a></li>
        <li><a href="/#proj">work</a></li>
        <li><a href="/about">about</a></li>
        <li><a href="/about#resume">resumé</a></li>
        <li><a href="https://prasadsanctuary.netlify.app/">3D</a></li>
    </div>
</div>



<style>
nav{
    z-index: 7;
}

li, a {
    text-decoration: none;
    color: var(--maintext);
    list-style-type: none;
    text-transform: uppercase;
    font-size: .9rem;
    font-weight: 500;
    transition: all 0.3s ease-in-out;
    z-index: 7;
}    
header{
    z-index: 7;
    display: flex;
    justify-content: space-between;
    align-items: center;  
    padding: 1% 7%;  
}
.logo{
    cursor: pointer;
    font-size: 1.2rem;
    font-weight: 500;
    color: #f1f1f1;
    
}
/* .nav-links{
    padding: 0;
    margin: 0;
} */
.nav-links li{
    display: inline-block;
    padding: .1rem 1.5rem;
    z-index: 7;
}

.nav-links li:hover{
    background-color: rgb(47, 51, 54);
    border-radius: 5px;
    z-index: 7;
} 


.resume{
    padding: 2px 20px;
    text-transform: uppercase;
}

.resume:hover{
    background-color: rgb(47, 51, 54);
    border-radius: 5px;
}

.menu{
    display: none;
    color: var(--textcolor);
}
.close{
    color: var(--textcolor);
}

/* ------------MOBILE MENU--------- */
.overlay{
        height: 100%;
        width: 0;
        position: fixed;
        z-index: 30;
        right: 0;
        top: 0;
        background-color: rgb(104, 104, 104);
        overflow-x: hidden;
        transition: all 0.2s ease 0s;
}
.overlay-content{
        display: flex;
        height: 100%;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        font-family: "Sora",sans-serif;
        font-weight: 200;
}
.overlay a{
        padding: 20px;
        font-size: 1.3rem;
        display: block;
        transition: all 0.4s ease 0s;
    }

.overlay .close{
        position: absolute;
        top: 1rem;
        right: 1.5rem;
        font-size: 30px;
}

/*---------------------- MEDIA QUERIES------------------ */
@media (max-width:700px){
    .nav-links{
        display:none;
    }
    .resume{
        display: none;
        text-transform: uppercase;
    }
    .menu{
        display: inherit;
        font-size:1.7rem;
        margin-bottom: -7px;
        z-index: 70;
    }

    .overlay{
        height: 100%;
        overflow: hidden;
        width: 0;
        position: fixed;
        z-index: 90;
        right: 0;
        top: 0;
        backdrop-filter: blur(5px);
        background-color: rgba(17, 17, 17, 0.945);
        transition: all 0.3s ease-in-out;
    }

    header{
       padding: 4% 7%;
    }

    
}

</style>



