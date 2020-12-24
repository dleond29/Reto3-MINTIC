
<template>
    <div class="container-fluid">
      <div class="row justify-content-center mb-2">
        <div class="col mt-5" v-for="(item, index) of team" :key="index">
          <team-card v-bind:member="item"></team-card>
        </div>
      </div>
    </div>
</template>

<script>
import TeamCard from "../components/TeamCard.vue";

export default {
  name: "App",
  components: {
    TeamCard,
  },
  data() {
    return {
      team: [
        {
          codigo: 1,
          nombre: "Diego León",
          descripcion: "Miembro equipo 8.",
          rol: "Desarrollador backend",
          image: "images/diegoL.png",
          tel: "3005677700",
          email: "diegoleon@correo.com"
        },
      ],
    };
  },
};
</script>

