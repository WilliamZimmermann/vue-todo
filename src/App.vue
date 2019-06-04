<template>
  <div>
    <h1>Vue TODO</h1>
    <label>
      Nova tarefa:
      <input autofocus type='text' @keyup.enter="addTask($event.target.value)">
    </label>
    <p>Minhas tarefas:</p>
    <ul>
      <li v-for="task in tasks">
        {{ task }}
      </li>
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
  },

  methods: {
    addTask: function(newTask){
      this.tasks.push(newTask);
    }
  }
}
</script>

<style lang="scss">
</style>
