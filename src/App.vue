<template>
  <div>
    <h1>Vue TODO</h1>
    <label>
      Nova tarefa:
      <input autofocus type='text'>
    </label>
    <p>Minhas tarefas:</p>
    <ul>
      <li>Estudar</li>
      <li>Correr</li>
      <li>Dormir</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      tasks: [
          'Estudar',
          'Correr',
          'Dormir',
          'Videogame',
      ]
    }
  }
}
</script>

<style lang="scss">
</style>
