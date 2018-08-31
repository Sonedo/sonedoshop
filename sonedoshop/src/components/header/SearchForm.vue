<template>
  <div class="search-form">
    <form>
      <div class="input-field">
        <input id="search" type="search" required>
        <label class="label-icon" for="search"><i class="material-icons">search</i></label>
        <i class="material-icons">close</i>
      </div>
    </form>
  </div>
</template>

<script>
  export default {
    name: 'SearchForm'
  }
</script>

<style scoped>
  .search-form {
    margin: 30px;
  }

</style>
