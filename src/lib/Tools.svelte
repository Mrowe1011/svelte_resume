<script>
    import { fade, blur, fly, slide, scale } from "svelte/transition";
    import { onMount } from 'svelte';

    let ready = false;
    onMount(() => ready = true);
</script>


{#if ready}
<div class="container">
<div in:fade class="block">
<h1>Coding Languages</h1>
<ul>
    <li>Python</li>
    <li>Jython</li>
    <li>Powershell</li>
    <li>Jenkins Groovy</li>
    <li>Powershell</li>
    <li>Javascript</li>
    <li>HTML</li>
    <li>CSS</li>
    <li>Integrated C</li>
</ul>
</div>

<div in:fade class="block">
    <h1>Software</h1>
    <ul>
        <li>GIT</li>
        <li>Jira</li>
        <li>Confluence</li>
        <li>Bitbucket</li>
        <li>GitLab</li>
        <li>Nexus Artifact Manager</li>
        <li>Artifactory Artifact Manager</li>
        <li>Jenkins</li>
        <li>Xebia Labs Release and Deploy</li>
        <li>Cisco Meraki</li>
        <li>Teamviewer</li>
    </ul>
</div>
<div in:fade class="block">
    <h1>Soft Skills</h1>
    <ul>
        <li>Autonomy</li>
        <li>Communication</li>
        <li>Adaptability</li>
        <li>Ethics</li>
    </ul>
</div>
</div>
{/if}
<style>
    @media only screen and (min-width: 513px) {
        .container {
            display: flex;
        }

        .block {
            flex: 1 1 0;
        }
    }

ul {
    list-style-type: none;
}
li {
    padding-top: 0.6%;
}
div {
    background-color:rgba(41, 41, 41, 0.679);
    padding: 1%;
    }
</style>