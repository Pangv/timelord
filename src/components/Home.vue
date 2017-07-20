<template lang="html">
<div class="row">
  <div class="col-sm-12 col-md-12 col-lg-12">
    <p>Hallo an welchen Projekten hast du heute gearbeitet?</p>
    <form action="">
      <div class="form-group">
        <label for="">Datum</label>
        <input disabled type="date" class="form-control" :value="days">
      </div>
    </form>
    <task v-for="(task,key, index) in tasks" :key="task.id" :text="task.text" :start="task.start" :end="task.end"></task>
    <button @click="addTask()" class="btn btn-default">
      <span class="glyphicon glyphicon-plus"></span>
    </button>
  </div>
</div>
</template>

<script>
import Task from './Task';

const moment = require('moment');

export default {
  name: 'home',
  data() {
    return {
      days: moment().format('YYYY-MM-DD'),
      newTask: '',
      tasks: [
        {
          text: 'Test',
          start: '00:00',
          end: '12:00',
        },
      ],
    };
  },
  components: {
    Task,
  },
  methods: {
    addTask() {
      this.tasks.push({
        text: this.newTask,
        start: moment().format('HH:mm'),
        end: '00:00',
      });
    },
    play() {

    },
    pause() {

    },
  },
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
