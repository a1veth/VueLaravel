<template>
  <div>
    <nav class="navbar navbar-expand-lg bg-dark" data-bs-theme="dark">
      <div class="container d-flex justify-content-between align-items-center">
        <!-- Home link -->
        <router-link :to="{ name: 'home' }" class="navbar-brand" style="font-weight: bold;">Home</router-link>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navbar items -->
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
            <li class="p-1 nav-item">
              <router-link
                :to="{ name: 'posts.index' }"
                class="nav-link active rounded bg-darkblue text-white px-3 py-2"
                aria-current="page"
              >
                Content
              </router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Render router view -->
    <router-view></router-view>
  </div>
</template>

<style scoped>
.bg-darkblue {
  background-color: #0d47a1; 
}
.nav-link:hover {
  background-color: #0b3a81; 
}
.nav-link {
  font-weight: bold;
}
</style>
