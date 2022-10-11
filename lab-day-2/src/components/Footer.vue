<template>
    <footer class="footer">
  <div class="content has-text-centered">
    <div>
        <img src=""/>
    </div>
    <div>
      <a>Contact Us</a>
      <a>Jobs</a>
      <a>Projects</a>
    </div>
    <div>
        <p>2972 Westheimer Rd. Santa Ana, Illinois 85486</p>
    </div>
    <div>
      <ul class="list">
        <li v-for="movie in movies">
        {{movie.title}} - {{movie.description}} - {{movie.content}}
        </li>
      </ul>
    </div>

  </div>
</footer>
</template>

<script setup>

const movies = [
    {
        title: 'Jurassic Park', 
        description: 'Action', 
        content: 'DVD',
    }, 
    {
        title: 'Ghost',
        description: 'Drama', 
        content: 'VHS'
    },
    {
        title: 'Back to the future',
        description: 'Sci-fi', 
        content: 'Blue Ray'
    }
]


</script>
<style scoped>
.list {
  list-style: none; 
  color: blue
}


</style>