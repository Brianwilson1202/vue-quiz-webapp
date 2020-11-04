<template>
  <b-container>
    <b-nav style="align-items: center" tabs>
      <b-nav-item disabled><b>Vue Quiz Game</b></b-nav-item>
      <b-nav-item disabled>Correct: {{ numCorrect }}</b-nav-item>
      <b-nav-item disabled>Total: {{ numTotal }}</b-nav-item>
      <b-nav-item>
        <b-button @click.prevent="reloadPage" variant="success">Restart</b-button>
      </b-nav-item>
    </b-nav>
  </b-container>
</template>

<script>
export default {
  props: ["numCorrect", "numTotal"],
  methods: {
  reloadPage(){
    window.location.reload()
  }
}
};
</script>
