<template>
  <div id="app">
    <nav class="navbar navbar-dark bg-dark">
      <div id="nav">
        <router-link to="/" class="nav-item nav-link active">Home</router-link>|
        <router-link to="/about" class="nav-item nav-link">About</router-link>
        <form class="form-inline">
          <input class="form-control mr-sm-2" type="text" placeholder="Username" />
          <input class="form-control mr-sm-2" type="password" placeholder="Password" />
          <button class="btn btn-primary" type="submit">Submit</button>
        </form>
      </div>
    </nav>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 2px;
}

#nav a {
  font-weight: bold;
  color: #42b983;
}

#nav a.router-link-exact-active {
  color: white;
}
</style>
