<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';
    export let keybank = 0;
    export let kent = 0;
    export let cohen = 0;
    export let riverside = 0;
    let ready = false;
    onMount(() => ready = true);
</script>

{#if ready}
<div>
    <div in:fly="{{ x: 200, duration: 500 }}" id="Keybank">
        <h1>Keybank DevOps Enginner Intern</h1>
        <h2>Jun 2022 - Aug 2022 (3 months)</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (keybank = 1)}>Job Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (keybank = 0)}> • </a></li>
            <li><a href="/" on:click|preventDefault={() => (keybank = 2)}>Tools I worked with</a></li>
        </ul>
        {#if keybank === 1}
        <p>
            Created value within the Continuous Integration and Deployment team at KeyBank by leveraging my knowledge of Python and GIT to create automated processes. I continuously learned new platforms to better enhance the development experience across the company’s development teams.
        </p>
        {:else if keybank === 2}
        <ul>
            <li>GIT</li>
            <li>Jira</li>
            <li>Confluence</li>
            <li>Python</li>
            <li>Jython</li>
            <li>Jenkin's Groovy</li>
            <li>Jfrog Artifactory</li>
            <li>Sonatype Nexus</li>
            <li>XebiaLabs Release</li>
            <li>XebiaLabs Deploy</li>
        </ul>
        {/if}
    </div>
    <hr in:fly="{{ x: 200, duration: 550 }}" >


    <div in:fly="{{ x: 200, duration: 600 }}"  id="Kent">
        <h1>Electronics Lab Lead Design and Innovation Hub Kent State</h1>
        <h2>Jan 2022 - Apr 2022 (4 months)</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (kent = 1)}>Job Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (kent = 0)}> • </a></li>
            <li><a href="/" on:click|preventDefault={() => (kent = 2)}>Tools I worked with</a></li>
        </ul>
        {#if kent === 1}
        <p>
            I revived the Electronics lab within Kent State’s Design and Innovation Hub from a place of inactivity to a functional lab by marketing it to both students and faculty across Kent’s campus.  I created value across departments by collaborating with the school of fashion to create electronics that can be sewed.
        </p>
        {:else if kent === 2}
        <ul>
            <li>Python</li>
            <li>Raspberry Pi's</li>
            <li>Integrated C</li>
            <li>Arduinos</li>
            <li>LillyPad Sewable Electronics</li>
            <li>Capacitors, Resistors, and other SMDs</li>
            <li>Voltera V-One PCB printer</li>
            <li>Multimeters</li>
            <li>3D Printing</li>
            <li>Fusion 360 3D Modeling</li>
        </ul>
        {/if}
    </div>
    <hr in:fly="{{ x: 200, duration: 650 }}" >

    <div in:fly="{{ x: 200, duration: 700 }}"  id="cohen">
        <h1>Cohen & Company Summer End User Technology Intern</h1>
        <h2>May 2021 - Aug 2021 (4 months)</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (cohen = 1)}>Job Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (cohen = 0)}> • </a></li>
            <li><a href="/" on:click|preventDefault={() => (cohen = 2)}>Tools I worked with</a></li>
        </ul>
        {#if cohen === 1}
        <p>
            I was entrusted to deploy, manage, and repair any user’s laptop or computer within the company. I created additional value by going beyond what was expected of me and created automation to streamline the windows deployment process.
        </p>
        {:else if cohen === 2}
        <ul>
            <li>PowerShell</li>
            <li>Jira</li>
            <li>Confluence</li>
            <li>Cisco Meraki</li>
            <li>Microsoft WDS, MDT</li>
            <li>Laptop Repair</li>
            <li>Windows Troubleshooting</li>
            <li>Teamviewer</li>
            <li>Office Standup</li>
        </ul>
        {/if}

    </div>
    <hr in:fly="{{ x: 200, duration: 750 }}" >

    <div in:fly="{{ x: 200, duration: 800 }}"  id="riverside">
        <h1>Riverside Local Schools IT Intern</h1>
        <h2>June 2018 - July 2020 (2 years 2 months)</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (riverside = 1)}>Job Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (riverside = 0)}> • </a></li>
            <li><a href="/" on:click|preventDefault={() => (riverside = 2)}>Tools I worked with</a></li>
        </ul>
        {#if riverside === 1}
        <p>
            I was entrusted to deploy, manage, and repair any user’s laptop or computer within the school district. I created additional value by going beyond what was expected of me and created automation to streamline the windows deployment process.
        </p>
        {:else if riverside === 2}
        <ul>
            <li>Batch Scripting</li>
            <li>Microsoft WDS, MDT</li>
            <li>Laptop Repair</li>
            <li>Windows Troubleshooting</li>
            <li>Teamviewer</li>
            <li>Office Standup</li>
        </ul>
        {/if}

    </div>
</div>
{/if}
<style>
    div {
    background-color:rgba(41, 41, 41, 0.679);
    padding: 1%;
    }
    ul.menu li{
        display : inline;
    }
    img {
        width: 50%;
        height: 80%;
        display: block;
        margin: auto;

    }

.menu {
    width: 100%;
    display: flex;
    padding: 0;
    list-style: none;

    text-align: center;
    
}
a, a:hover, a:active, a:visited {
     color: white;
 }

 .dot {
     margin-left: 1%;
     margin-right: 1%;
 }
</style>