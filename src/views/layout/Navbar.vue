<template>
  <div>
    <section class="section_1 container-fluid p-0">
      <div class="d-flex flex-column">
        <header>
          <div>
            <b-navbar toggleable="lg" type="dark" variant="info">
              <b-navbar-brand>ASTIG</b-navbar-brand>

              <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

              <b-collapse id="nav-collapse" is-nav>
                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">
                  <b-navbar-nav>
                    <b-nav-item href="/dataentry">Data Entry</b-nav-item>
                    <b-nav-item href="/fileupload">File Upload</b-nav-item>
                  </b-navbar-nav>
                  <b-nav-item-dropdown right>
                    <!-- Using 'button-content' slot -->
                    <template #button-content>
                      <em>User</em>
                    </template>
                    <b-dropdown-item href="#">Profile</b-dropdown-item>
                    <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                  </b-nav-item-dropdown>
                </b-navbar-nav>
              </b-collapse>
            </b-navbar>
          </div>
        </header>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>
