<template lang="html">
<div class="row">
  <div class="col-sm-12 col-md-12 col-lg-12">
    <p>Hallo an welchen Projekten hast du heute gearbeitet?</p>

<form action="">
  <div class="form-group">
    <label for="">Datum</label>
    <input disabled type="date" class="form-control">
  </div>
</form>
    <form action="">

      <div class="form-group">
        <label for="">Projekttitel / Aufgabe</label>
        <input type="text" class="form-control" placeholder="BK-Strategie">
      </div>
      <div class="form-group">
        <label for="">Anfangszeit</label>
        <input type="time" class="form-control">
      </div>
      <div class="form-group">
        <label for="">Endzeit</label>
        <input type="time" class="form-control">
      </div>
      <button class="btn btn-default">
        <span class="glyphicon glyphicon-play"></span>
      </button>
      <button class="btn btn-default">
        <span class="glyphicon glyphicon-pause"></span>
      </button>
      <button class="btn btn-default">
        <span class="glyphicon glyphicon-pencil"></span>
      </button>
    </form>

    <button class="btn btn-default">
      <span class="glyphicon glyphicon-plus"></span>
    </button>
  </div>

</div>
</template>

<script>
export default {
  name: 'home',
};
</script>

<style lang="css" scoped>
  form {
    margin-bottom: 2rem;
  }

  .form-group {
    display: inline-block;
  }
</style>
