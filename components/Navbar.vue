<template>
    <nav class="navbar is-black" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a @click="toggle" role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbar">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>
      <div id="navbar" class="navbar-menu">
        <div class="navbar-end">
          <a id="resume" class="navbar-item" href="/pdf/resume.pdf" title="resume">resume</a>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
  name: 'Navbar',
  methods: {
    toggle (event) {
      const className = 'is-active';
      event.target.classList.toggle(className);
      const navbar = document.getElementById('navbar');
      navbar.classList.toggle(className)
    }
  }
}
</script>