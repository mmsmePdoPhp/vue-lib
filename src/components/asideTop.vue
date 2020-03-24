<template>
  <div>
    <b-card no-body style="max-width: 20rem;">
      <template v-slot:header>
        <h4 class="mb-0">Hello World</h4>
      </template>

      <b-card-body>
        <b-card-text>
          <b-list-group flush >
            <b-list-group-item>
              <b-form-group>
                <template v-slot:label></template>

                <b-form-checkbox-group 
                  id="flavors"
                  v-model="selected"
                  :options="flavours"
                  name="flavors"
                  class="ml-4"
                  aria-label="Individual flavours"
                  stacked
                ></b-form-checkbox-group>
              </b-form-group>
            </b-list-group-item>
          </b-list-group>
        </b-card-text>
      </b-card-body>

      <b-card-footer>This is a footer</b-card-footer>
    </b-card>
  </div>
</template>


<script>
export default {
  data() {
    return {
      flavours: [
        "برنامه نویسی وب",
        "برنامه نویسی موبایل",
        "برنامه نویسی دستکتاب",
        "برنامه نویسی پایگاه داده",
        "Very Berry"
      ],
      selected: [],
      allSelected: false,
      indeterminate: false
    };
  }
};
</script>


<style lang="scss" scoped>

</style>