<script>
  import { onMount } from 'svelte'
  let posts = []
  
  onMount(async ()=>{
    const response = await fetch("https://ipapi.co/json/")
    posts = await response.json()
    console.log(posts.ip)
  })


</script>

<h1>
hello {posts.ip}
</h1>

