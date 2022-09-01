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
        <p>I was on the CI/CD team at Keybank's Devops department. Our team was spearheading the transition to the Google Cloud Platform while also migrating our current GIT provider from bitbucket to GitLab. My main task was migrating development artifacts from Sonatype Nexus to Jfrog Artifactory.  I was moving both files and helping transition development processes like Jenkins jobs and XebiaLabs release jobs. I also got to sit in on much of the GCP transition and got to see how Ansible was deployed to the cloud. While I was waiting for development teams I spent my time developing python tools that could save the team time in the future. Finally, I solved a long standing issue and optimized an old jython file that generated the stages of a deployment in XLR. The problem the team faced was that the file could not exceed 100kb so I learned how the script worked and split it into 2 files and imported functions as needed.</p>
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
        <p>During the school year I took an interest in my university’s soldering lab to work on some of my projects. After expressing interest in the lab, I was offered a position to run it since it had been left vacant for 6 months. I took it from a place of inactivity to a functioning lab used by students and faculty. I set up the lab in accordance to fume extraction and safety rules. I gave life back to the lab by reaching out to Kent professors to create workshops for students within the lab. I also created a doorbell to send an alert to Microsoft Teams when someone entered the door.</p>
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
        <p>My main duties were imaging laptops for new and existing users and then assisting them with anything they needed. This includes hardware, software, and even general tech advice. I had other auxiliary duties in this role like creating and maintaining organization systems for storage rooms, creating PowerShell scripts to ease imaging, and documenting fix processes to create knowledge base articles. I was also selected to travel to a new office and assist with its standup over the course of three days. In this position I was paired with another intern and two people who oversaw me.</p>
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
        <p>My duties in this position gradually built up over time as I progressed through my internship. I started with learning how to fix hardware. This included fixing things like Chrome Books, Windows laptops, and Windows desktops. I would do everything from replacing motherboards to something as simple as replacing keys. After learning hardware skills, I was taught software skills like how to image PCs through windows deployment services and general troubleshooting for programs we used like SMART and other educational software. After I had these two foundational skills mastered, I started completing tickets like a normal break fix tech would. I assisted users and explained to them what I was doing in a way that made it understandable to them. After I became familiar with general end user ticketing, I started getting assigned networking tasks. One of my first projects was setting up a PC lab for design students. I ran cables and worked with an upper-level tech to configure a Cisco switch for the room. Towards the end of my internship, I began working on creating a Windows 10 image for our computers with Microsoft Deployment Toolkit on their Windows 2006 server running WDS.</p>
        {:else if riverside === 2}
        <ul>
            <li>Batch</li>
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