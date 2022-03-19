<template>
  <v-card color="basil">
    <v-card-title class="text-center justify-center py-6">
      <h1 class="tes">
        NOS VALEURS
      </h1>
    </v-card-title>

    <v-tabs v-model="tab" background-color="transparent" grow>
      <v-tab v-for="item in items" :key="item">
        {{ item.title }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item">
        <v-card flat>
          <v-card-text>{{ item.text }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>
<script>
export default {
  data() {
    return {
      tab: null,
      items: [
        {
          title: " SATISFACTION",
          text:
            "LE PLAISIR QU’ÉPROUVE NOTRE CLIENTÈLE A VENIR PARTAGER AVEC NOS INSTRUCTEURS QUALIFIÉS EST UN FACTEUR CLÉ DE NOTRE RÉUSSITE. UN CLIENT SATISFAIT SERA UN PARTENAIRE AVEC LEQUEL NOUS DÉVELOPPERONS UNE RELATION DURABLE. "
        },
        {
          title: "DÉCOUVERTE",
          text:
            "FAIRE DÉCOUVRIR DES SPORTS EN ÉMERGENCE, DES TECHNIQUES ET DES LIEUX EXCEPTIONNELS DANS NOTRE RÉGION POUR ASSURER UNE EXPÉRIENCE HORS DE L'ORDINAIRE A NOTRE CLIENTÈLE "
        },
        {
          title: " RESPONSABILITÉ ",
          text:
            "NOUS SOUHAITONS PARTAGER NOS CONNAISSANCES ET FAIRE BRILLER LE DÉVELOPPEMENT ENTREPRENEURIALE EN INTÉGRANT CERTAINES PRÉOCCUPATION SOCIALES, ENVIRONNEMENTALES ET ECONOMIQUES A NOTRE CULTURE D'ENTREPRISE"
        }
      ]
    };
  }
};
</script>

<style>
.basil--text {
  color: #2196f3 !important;
}
.tes {
  font-family: "Shizuru", cursive;
}
</style>
<style>
@import url("https://fonts.googleapis.com/css2?family=Shizuru&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Supermercado+One&display=swap");
</style>
