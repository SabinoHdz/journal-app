<template>
  <div class="entry-container mb-3 pointer p-2">
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">15</span>
        <span class="mx-1 fs-5">Julio</span>
        <span class="mx-2 fw-light">2023,lunes</span>
    </div>
    <div class="entry-description">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Mollitia, dolores ab? Dolor incidunt unde sapiente necessitatibus recusandae, ducimus pariatur rerum reiciendis aut? Voluptatum sapiente velit ad odit dolorum reiciendis magnam.
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.entry-container{
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;
    &:hover{
        background-color: lighten($color: grey, $amount: 45);
    }
    .entry-description{
        font-size: 12px;
    }
}

</style>