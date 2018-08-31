<template>
  <div>
    <nav class="nav-extended">
      <div class="nav-wrapper">
        <a href="#" class="brand-logo">Logo</a>
        <ul class="right hide-on-med-and-down">
          <li><SearchForm/></li>
          <li><UserProfile/></li>
        </ul>
      </div>
      <div class="nav-content">
        <ul id="dropdown1" class="dropdown-content">
          <li><a href="#!">one</a></li>
          <li><a href="#!">two</a></li>
          <li class="divider"></li>
          <li><a href="#!">three</a></li>
        </ul>
        <ul class="tabs tabs-transparent">
          <li class="tab"><router-link to="/">Home</router-link></li>
          <li class="tab"><a class="dropdown-trigger" href="#!" data-target="dropdown1">Dropdown</a></li>
          <li class="tab">Labels</li>
          <li class="tab">Browse</li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
  import SearchForm from './SearchForm.vue'
  import UserProfile from './UserProfile.vue'
  import GenresDropdown from './GenresDropdown.vue'
  export default {
    name: 'AppHeader',
    components: {
      SearchForm, UserProfile, GenresDropdown
    },
    mounted(){
      $(".dropdown-trigger").dropdown();
    }
  }
</script>

<style scoped>

</style>
