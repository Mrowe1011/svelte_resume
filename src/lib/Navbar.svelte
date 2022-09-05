<script>
	import Work from "./Work.svelte";
	import Tools from "./Tools.svelte";
    import Volunteer from "./Projects.svelte"
    import Clubs from "./clubs.svelte";
    import Education from "./Education.svelte";
    export let menu = 1;
</script>

<div id="Introduction">
    
    <div>
        <div id="whoami">
            <h1>Hello.</h1>
            <h2>My name is Kevin Bahner.</h2>
        </div>

        <h4 id="socials"> <a href = "mailto: kevbahner@gmail.com" target="_blank">kevbahner@gmail.com</a> | <a href="https://www.linkedin.com/in/kevin-bahner-b313641a2/" target="_blank">LinkedIn</a> | <a href="https://github.com/Mrowe1011" target="_blank">GitHub</a></h4>

    </div>

    <hr>
        <div id="navbar">
            <ul id="menu">
                <li><a href="/" on:click|preventDefault={() => (menu = 1, gtag('event', 'Navigation', {'navagate to':'Work Experience'}))}>Work Experience</a></li> 
                <li><a href="/" on:click|preventDefault={() => (menu = 5, gtag('event', 'Navigation', {'navagate to':'Education'}))}>Education</a></li>
                <li><a href="/" on:click|preventDefault={() => (menu = 2, gtag('event', 'Navigation', {'navagate to':'Skills'}))}>Skills</a></li>
                <li><a href="/" on:click|preventDefault={() => (menu = 3, gtag('event', 'Navigation', {'navagate to':'Projects'}))}>Projects</a></li>
                <li><a href="/" on:click|preventDefault={() => (menu = 4, gtag('event', 'Navigation', {'navagate to':'Clbus'}))}>Clubs</a></li>
            </ul>
        </div>
        <hr>
</div>


{#if menu === 1}
<Work />
{:else if menu === 2}
<Tools />
{:else if menu === 3}
<Volunteer />
{:else if menu === 4}
<Clubs />
{:else if menu === 5}
<Education />
{/if}



<style>
#socials {
    font-weight: 400;
    padding-bottom: 0.4%;
}
#whoami {
    padding-top: 0;
    padding-bottom: 0;

}
#whoami h1 {
font-size: 6em;
font-weight: lighter;
padding: 0;
margin-bottom: 0;
}

#whoami h2 {
font-size: 2em;
font-weight: lighter;
margin-top: 0;
}
a, a:hover, a:active, a:visited {
     color: white;
     
     
 }
#navbar {
    margin-left: 8%;
    margin-right:8%;
    margin-top: 0;
    margin-bottom: 0;

}
#Introduction {
    background-color:rgba(41, 41, 41, 0.679);
    padding: 1%;
    
}
ul#menu li{
		display : inline;
	}
#menu a {
    text-decoration: none;
    font-size: 0.8em;
}

#menu {
    width: 100%;
    display: flex;
    padding: 0;
    list-style: none;
    justify-content:space-between;
    text-align: center;
    
}

</style>