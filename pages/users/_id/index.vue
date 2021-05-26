<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate(data) {
    //check if the id is numeric value (while URL is loaded)
    return /^\d+$/.test(data.params.id);
  }
}
</script>
