<template>
  <div id="div">
    <h2>Home Page</h2>

    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci aut quidem vel voluptatem! Corporis deserunt eligendi quia soluta. Adipisci aliquam consectetur cum deserunt ea iure laudantium quas qui ratione rem, velit, voluptatibus? Amet aperiam error fugiat illum magni maxime molestiae, necessitatibus odio officiis, possimus quibusdam, quo reiciendis sint sunt tempore.</p>
    <router-link to="/todos">Todos</router-link>
  </div>
</template>

<style>
a {
  color: #fff;
  padding: 10px 20px;
  background: rgb(212,75,56);
  border-radius: 8px;
  text-decoration: none;
}
a:hover {
  background: rgb(232,95,76);
}
a:active {
  background: rgb(232,95,76);
}
#div {
  width: 80%;
  margin: 60px auto;
}
p {
  font-weight: 500;
  font-size: 18px;
  color: #2c3e50;
}

</style>