<template lang="html">
  <div class="row">
    <h1>Mein Profil</h1>
    <form action="">
      <div class="form-group">
        <label for="">User</label>
        <input disabled type="text" class="form-control" placeholder="User">
      </div>
      <div class="form-group">
        <label for="">Name</label>
        <input disabled class="form-control" type="text" name="" value="" placeholder="Nachname">
      </div>
      <div class="form-group">
        <label for="">Vorname</label>
        <input disabled class="form-control" type="text" name="" value="" placeholder="Vorname">
      </div>
      <button class="btn btn-default" type="submit" name="button">Speichern</button>
      <button class="btn btn-default">Felder freischalten</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'hi',
    };
  },
  methods: {
    update() {
      return this.message;
    },
  },
};
</script>

<style lang="css" scoped>

</style>
