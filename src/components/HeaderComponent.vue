<template>
   <header>
      <nav class="general-nav">
         <ul class="general-menu">
            <RouterLink to="/">Главная</RouterLink>
            <RouterLink to="/roms">Образы игр</RouterLink>
            <RouterLink to="/articles">Статьи</RouterLink>
            <RouterLink to="/search">Поиск</RouterLink>
            <li><a href=""></a></li>
         </ul>
      </nav>
   </header>
</template>

<script setup lang="ts">

</script>

<style scoped>
header {
   width: 1800px;
   margin-inline: auto;
}
.general-nav {
   width: 80%;
   padding: 20px;
}
.general-menu {
   display: flex;
   justify-content: space-between;
   list-style: none;
}
.general-menu a {
   text-decoration: none;
   font-size: 18px;
   font-variant: small-caps;
   text-transform: uppercase;
}
</style>