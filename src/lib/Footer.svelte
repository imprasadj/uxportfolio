<script>

</script>

<div class="footer" id="footerbg">
    <div class="footerbox">

        <div class="left">
            <h3>DESIGN & BUILD<br/>  <span>Prasad Jadhav</span></h3> 
        </div>
            
        <div class="right">
            <h3>SOCIALS<br/>  
                <span>
                    <a target="_blank" href="https://twitter.com/prasadjux">Twitter</a>
                    <a target="_blank" href="https://www.linkedin.com/in/prasad-1feb97/">LinkedIn</a>
                    <a target="_blank" href="https://unsplash.com/@prasadjadhav">Unsplash</a>
                </span>
            </h3>
                
        </div>

    </div>
    
</div>

<style>
#footerbg{
    z-index: -1;
}
.footer{
    
    width:100%;
    height: 11rem;
    bottom: 0;
    background-color: var(--bgcolor);
    padding: 7rem 0 2rem 0;
    
}

.footerbox{
    padding: 0 7% 0 7%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    z-index: 10;
}

.left{
    display: flex;
    align-items:flex-start;
    z-index: 10;
}

.right{
    display: flex;
    justify-content: flex-end;
    z-index: 10;
}


h3{
font-family: "Syne", sans-serif;
font-size: .7rem;
color: var(--sectext);
}

span{
    font-size: 1.4rem;
    text-transform: uppercase;
    color: var(--maintext);
}


.right h3{
    text-align: right;
}

.right a{
    font-size: .9rem;
    margin-left:.5rem;
    text-transform: uppercase;
    color: var(--sectext); 
}

.right a:hover{
    color: var(--maintext);
}


@media (max-width:800px){



.footerbox{
    padding: 0 10%;
    display: grid;
    grid-template-columns: 1fr;
}

.right{
    display: flex;
    justify-content: flex-start;
}

.right h3{
    text-align: left;
}

.right a{
    font-size: .8rem;
    margin: 0 1rem 0 0;
    text-transform: uppercase;
    color: rgb(170, 170, 170); 
}

.right a:hover{
    color: var(--textcolor);
}

}
</style>