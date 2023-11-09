<template>
  <v-container>
    <v-row class="text-center">


      <h1 >Sofia Rocha - Programadora Full-Stack</h1>

      <p>
         Sou programadora full-stack com 1 ano de experiência no mercado de trabalho.

      </p>
      <h2>Algumas tecnologias com que já trabalhei</h2>
      <ul>
        <li v-for="item in items" :key="item.id">
          {{item.message}}
        </li>
      </ul>
    </v-row>
  </v-container>
</template>

<script>

import { ref } from "vue";





export default {
  name: "HelloWorld",

  setup(){
    const items = ref([{ message: 'Python' },
      { message: 'Java' },
      { message: 'HTML5' },
      { message: 'CSS3' },
      { message: 'PHP' },
      { message: 'JavaScript' },
      { message: 'Sass' },
      { message: 'Laravel' },
      { message: 'Angular' },
      { message: 'React' },
      { message: 'Django' },
      { message: 'CodeIgniter' }]);

    return {
      items
    };
  }

};

</script>
