<template>
  <div>
    <nav class="navbar navbar-dark sticky-top bg-blue flex-md-nowrap p-0">
      <nuxt-link class="navbar-brand col-sm-3 col-md-2 mr-0" to="/">Company name</nuxt-link>
      <ul class="navbar-nav px-3">
        <li class="nav-item text-nowrap">
          <a class="nav-link" href="#">Sign out</a>
        </li>
      </ul>
    </nav>
    <nuxt-link to="/">Home</nuxt-link>
    &nbsp;
    <nuxt-link to="/inspire">Inspire</nuxt-link>
    
    <div class="container-fluid">
      <div class="row">
        <nav class="col-md-2 d-none d-md-block bg-light sidebar">
          <div class="sidebar-sticky">
            <h6 class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted">
              <span>Menu</span>
              <a class="d-flex align-items-center text-muted" href="#">
                <span data-feather="plus-circle"></span>
              </a>
            </h6>
            <ul class="nav flex-column mb-2">
              <li class="nav-item">
                <nuxt-link class="nav-link" to="/">Dashboard</nuxt-link>
              </li>
              <li class="nav-item">
                <nuxt-link class="nav-link" to="/inspire">Inspire</nuxt-link>
              </li>
            </ul>
          </div>
        </nav>

        <main role="main" class="col-md-9 ml-sm-auto col-lg-10 pt-3 px-4">
          <nuxt />
        </main>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'default'
}
</script>
