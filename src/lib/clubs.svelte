<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';
    let ready = false;
    onMount(() => ready = true);
    export let robot = 0
    export let provost = 0

</script>

{#if ready}

<div>
    <div in:fly="{{ x: 200, duration: 500 }}" id="provost">
        <h1>Provost Leadership Academy, Mentor</h1>
        <h2>2020 - Present</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (provost = 1)}>Club Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (provost = 0)}> • </a></li>
            <li><a href="https://www.kent.edu/success/pla" target="_blank">Learn More</a></li>
        </ul>
        {#if provost === 1}
        <div>
        <p>The Provost Leadership Academy gives freshman a chance to make a real impact on their own campus by giving them the ability to present an issue and solution to the Provost of Kent State University. I have participated in the Provost Leadership Academy for two years. During my first year as a mentee, I created a tutorial on how to use a new classroom tool that we would be transitioning to for the next school year. The tutorial I helped create was implemented and suggested to all Kent students for the first few months of using the new tool. After my first year I was invited to become a mentor for incoming freshmen next year. The following year I gave my group of 10 freshmen the tools and encouragement they needed to make a great project. They chose to reopen a bowling alley on campus that had been shut down a little bit before COVID happened. I helped them create a financial break down and five-year plan of reopening the bowling alley. We received a first-place award at the Kent State Research Symposium for community outreach and recreation. </p>
        <img src='./images/mentees.jpg' alt="My mentees!">
        </div>
        {/if}
    </div>
    <hr in:fly="{{ x: 200, duration: 550 }}">
    <div in:fly="{{ x: 200, duration: 600 }}" id="robot">
        <h1>Robot Fighting, Team Leader</h1>
        <h2>August 2015- July 2019</h2>
        <ul class="menu">
            <li><a href="/" on:click|preventDefault={() => (robot = 1)}>Club Description </a></li> 
            <li class="dot"><a href="/" on:click|preventDefault={() => (robot = 0)}> • </a></li>
            <li><a href="https://thinkmfg.com/robobots/" target="_blank">Learn More</a></li>
        </ul>
        {#if robot === 1}
        <p>Built metal RC cars with weapons on them. Competed against other schools in the final tournament. The program is very similar to the TV Show “Robot Wars.” </p>
        {/if}
    </div>

</div>

{/if}

<style>
h2 {   
    font-weight: lighter;
}
    img {
        width: 50%;
        height: 80%;
        display: block;
        margin: auto;

    }
    div {
    background-color:rgba(41, 41, 41, 0.679);
    padding: 1%;
    }
    ul.menu li{
        display : inline;
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