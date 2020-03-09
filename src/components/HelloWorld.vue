<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo-oasis.png')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Bienvenidos al Hotel Oasis
        </h1>

        <p class="subheading font-weight-regular">
          Visítanos para una experiencia única
          <a href="Reservation.vue" target="_blank"
            >Reserva aquí</a
          >
        </p>
      </v-col>

      <v-col class="mb-5" cols="12">
        <h2 class="headline font-weight-bold mb-3">
          Redes Sociales
        </h2>

        <v-row justify="center">
          <a
            v-for="(next, i) in socialMedia"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "HelloWorld",

  data: () => ({
    socialMedia: [
      {
        text: "Instagram",
        href: "#"
      },
      {
        text: "Facebook",
        href: "#"
      },
      {
        text: "Twitter",
        href: "#"
      }
    ]
  })
};
</script>
