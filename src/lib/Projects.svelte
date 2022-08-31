<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';
    let ready = false;
    onMount(() => ready = true);
    export let website = 0
    export let doorbell = 0
    export let aws = 0
</script>

{#if ready}

<div>
    <div in:fly="{{ x: 200, duration: 500 }}" id="website">
        <h1>This website!</h1>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (website = 1)}>Project Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (website = 0)}> • </a></li>
            <li><a href="https://github.com/Mrowe1011/svelte_resume">Github</a></li>
        </ul>
        {#if website === 1}
        <p>This website was built from scratch using the Svelte Javascript framework. Check out my GitHub page to see my progress as I was developing the website.</p>
        {/if}
    </div>


    <hr in:fly="{{ x: 200, duration: 550 }}">


    <div in:fly="{{ x: 200, duration: 600 }}" id="doorbell">
        <h1>Raspberry Pi Doorbell</h1>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (doorbell = 1)}>Project Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (doorbell = 0)}> • </a></li>
            <li><a href="https://github.com/Mrowe1011/doorbell">Github</a></li>
        </ul>
        {#if doorbell === 1}
        <p>While working at the Design and Innovation’s electronics lab I solved a standing issue they had of not knowing when people came into the space. I leveraged a Raspberry Pi, laser, Light Dependent Resistor, Python, and a Microsoft teams API to send a message to a MS teams channel every time a person broke the laser’s beam. Check out the GIT repository to see how it works!</p>
        {/if}
    </div>


    <hr in:fly="{{ x: 200, duration: 650 }}">

    <div in:fly="{{ x: 200, duration: 700 }}" id="aws">
        <h1>Free AWS VPN</h1>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (aws = 1)}>Project Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (aws = 0)}> • </a></li>

        </ul>
        {#if aws === 1}
        <p>While looking for a VPN I came across an amazon EC2 instance that was free and able to run an OpenVPN instance in AWS. I was able to configure and setup my Linux container through SSH so that I was able to use it just like a consumer VPN.</p>
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
.menu a {

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