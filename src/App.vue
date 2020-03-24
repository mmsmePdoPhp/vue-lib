<template>
  <div id="app">
    <b-container fluid class="p-0">

        <b-navbar type="dark" class="d-flex flex-row-reverse p-0" variant="light">
          
          <b-navbar-brand href="#" class="h3 text-dark  m-0 px-2 m-auto">
            <b-icon icon="book"></b-icon>
          </b-navbar-brand>

            <b-input-group class="d-flex align-items-center max-width m-auto">
              <b-input-group-prepend class="d-flex">
                  <b-button variant="outline-success" >
                    <b-icon icon="search"></b-icon>
                  </b-button>
              </b-input-group-prepend>

              <b-form-input class="" type="text"></b-form-input>
            </b-input-group>


         <b-dropdown text="در باره ما" class="mr-auto">
          <b-dropdown-item href="#">An item</b-dropdown-item>
          <b-dropdown-item href="#">Another item</b-dropdown-item>
      </b-dropdown>

        </b-navbar>
    </b-container>

      <div id="nav">
        <router-link to="/">Home</router-link>|
        <router-link to="/about/10">About</router-link>
      </div>
      <router-view />
  </div>
</template>

<style lang="scss" scoped>
.max-width{
  max-width: 300px;
}
</style>
