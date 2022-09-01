<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';
    let ready = false;
    onMount(() => ready = true);
</script>

{#if ready}

<div>
    <div in:fly="{{ x: 200, duration: 500 }}" id="provost">
        <h1>Kent State University</h1>
        <h2>BBA, Computer Information Systems | Associate of Arts | 3.96 GPA</h2>
        <h3>Expected Graduation: May 2023 </h3>
    </div>
    <hr in:fly="{{ x: 200, duration: 550 }}">
    <div in:fly="{{ x: 200, duration: 600 }}" id="provost">
        <h1>Riverside High School</h1>
        <h2>Lakeland CCP and Honors Classes | Honors Diploma | 3.6 GPA</h2>

    </div>

</div>

{/if}

<style>

    h2,h3 {
        font-weight: lighter;

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