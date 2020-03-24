<template>
  <b-navbar type="light" toggleable="sm" class="d-flex flex-row-reverse p-0" variant="light">
    <b-collapse id="nav-collapse-top" class="d-flex flex-row-reverse" is-nav>
      <div class="rtl">
        <!-- Image and text -->
        <b-navbar variant="faded" class="logo" type="light">
          <b-navbar-brand href="#" class="text-light">
            <b-icon icon="book"></b-icon>&nbsp; EEB
          </b-navbar-brand>
        </b-navbar>
      </div>

      <b-input-group class="d-flex align-items-center max-width m-auto">
        <b-input-group-prepend class="d-flex">
          <b-button variant="outline-success">
            <b-icon icon="search"></b-icon>
          </b-button>
        </b-input-group-prepend>

        <b-form-input class="rtl search" type="text" placeholder="کتابتو  پیدا کن ..."></b-form-input>
      </b-input-group>

      <b-nav-item-dropdown
        text="ورود / ثبت نام"
        variant="outline-primary"
        class="mr-auto d-none d-sm-block"
      >
        <b-dropdown-item href="#">ورود</b-dropdown-item>
        <b-dropdown-item href="#">ثبت نام</b-dropdown-item>
      </b-nav-item-dropdown>

      <b-nav-item-dropdown text="Lang" class="list-unstyled" right>
        <b-dropdown-item href="#">EN</b-dropdown-item>
        <b-dropdown-item href="#">ES</b-dropdown-item>
        <b-dropdown-item href="#">RU</b-dropdown-item>
        <b-dropdown-item href="#">FA</b-dropdown-item>
      </b-nav-item-dropdown>

      <b-nav-item-dropdown text="در باره ما" class="mr-auto d-none d-sm-block">
        <b-dropdown-item href="#">درباره ما</b-dropdown-item>
        <b-dropdown-item href="#">تماس با ما</b-dropdown-item>
      </b-nav-item-dropdown>

      <b-navbar-toggle target="nav-collapse-top-top" class="p-0">
        <b-dropdown text="در باره ما" class="mr-auto">
          <b-dropdown-item href="#">An item</b-dropdown-item>
          <b-dropdown-item href="#">Another item</b-dropdown-item>
        </b-dropdown>
      </b-navbar-toggle>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {};
</script>


<style lang="scss" scoped>
.max-width {
  max-width: 500px;
}
.rtl {
  direction: rtl;

}
.logo{
  background-color: rgb(107, 25, 78);
}
.search{
  
  align-content: center;
  background-color: rgba(240, 173, 50, 0.623);
}
</style>