<script>
	import Work from "./Work.svelte";
	import Tools from "./Tools.svelte";
    import Volunteer from "./Volunteer.svelte"

    export let menu = 1;
</script>

<div id="Introduction">
    
    <div>
        <h1>Kevin Bahner</h1>
        <h4> <a href = "mailto: kevbahner@gmail.com">kevbahner@gmail.com</a> | <a href="https://www.linkedin.com/in/kevin-bahner-b313641a2/">Visit my LinkedIn!</h4>
            <hr>
        </div>
        <div id="navbar">
            <ul id="menu">
                <li><a href="/" on:click|preventDefault={() => (menu = 1)}>Work Expirence</a></li> 
                <li><a href="/" on:click|preventDefault={() => (menu = 2)}>Tooling Expirence</a></li>
                <li><a href="/" on:click|preventDefault={() => (menu = 3)}>Volunteer Activities</a></li>
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
{:else}
<h1>
	Page Not Found
</h1>
{/if}



<style>
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