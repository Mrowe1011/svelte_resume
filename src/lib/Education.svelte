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
        <h1>Google Cloud Digital Leader Certification</h1>
        <h2>Issued Sep 2022 - Expires Sep 2025</h2>
        <h3>Credential ID: <a href="https://www.credential.net/816a074b-3494-4f89-9b32-19b874c7ecb5">58098342</a></h3>

    </div>
    <hr in:fly="{{ x: 200, duration: 650 }}">
    <div in:fly="{{ x: 200, duration: 700 }}">
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
    a, a:hover, a:active, a:visited {
     color: white;
 }

</style>