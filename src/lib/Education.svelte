<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';
    let ready = false;
    onMount(() => ready = true);
</script>

{#if ready}

<div>
    <div in:fly="{{ x: 200, duration: 500 }}">
        <h1>Kent State University</h1>
        <h2>BBA, Computer Information Systems | Associate of Arts | 3.96 GPA</h2>
        <h3>Expected Graduation: May 2023 </h3>
    </div>
    <hr in:fly="{{ x: 200, duration: 550 }}">
    <div in:fly="{{ x: 200, duration: 600 }}">
        <h1>Riverside Highschool</h1>
        <h2>Lakeland College Credit Plus and Honors Classes | Honors Diploma | 3.6 GPA</h2>

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

</style>