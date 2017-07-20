<template lang="html">
  <form action="">
    <div class="form-group">
      <label for="">Projekttitel / Aufgabe</label>
      <input type="text" class="form-control" placeholder="BK-Strategie" :value="text">
    </div>
    <div class="form-group">
      <label for="">Anfangszeit</label>
      <input type="time" class="form-control" :value="start">
    </div>
    <div class="form-group">
      <label for="">Endzeit</label>
      <input type="time" class="form-control" :value="end">
    </div>
    <span class="pull-right">
      <button class="btn btn-default">
          <span class="glyphicon glyphicon-play"></span>
      </button>
      <button class="btn btn-default">
         <span class="glyphicon glyphicon-pause"></span>
       </button>
      <button class="btn btn-default">
          <span class="glyphicon glyphicon-pencil"></span>
      </button>
      <button class="btn btn-default">
        <span class="glyphicon glyphicon-trash"></span>
      </button>
    </span>
  </form>
</template>

<script>
export default {
  name: 'task',
  props: ['text', 'start', 'end'],
  data() {
    return {

    };
  },
};
</script>

<style lang="css" scoped>
form {
  padding: .5rem 1rem;
  border: 1px solid #ccc;
  background-color: #ccc;
  border-radius: 4px;
}

.pull-right {
  margin-top: 2.5rem;
}

.form-group {
  display: inline-block;
}

</style>
