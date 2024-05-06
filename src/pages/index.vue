<script setup lang="ts">
import { MaisonRecord } from '@/types';
import { MaisonRecord } from '@/pocketbase-types';

const maisonsListe: MaisonRecord[] = [
    {
    "adresse": "10 Avenue de la Plage , Avignon 84000",
    "collectionId": "iiey60bvm8pv197",
    "collectionName": "maison",
    "created": "2024-04-12 07:09:53.565Z",
    "favori": true,
    "id": "5ehui2o0c8duc3p",
    "image": "maison_bord_mer_9QRjc7NMUK.jpeg",
    "nbChambres": 5,
    "nbSdb": 3,
    "nomMaison": "Maison en Bord de Mer",
    "prix": 750000,
    "surface": 300,
    "updated": "2024-04-12 07:09:53.565Z"
  },
  {
    "adresse": "20 Chemin des Champs , Rochefourchat 26340",
    "collectionId": "iiey60bvm8pv197",
    "collectionName": "maison",
    "created": "2024-04-12 07:13:03.339Z",
    "favori": false,
    "id": "3kxp283fzfp1lbv",
    "image": "maison_campagne_2FqyzOWrwq.webp",
    "nbChambres": 4,
    "nbSdb": 2,
    "nomMaison": "Maison de Campagne",
    "prix": 500000,
    "surface": 250,
    "updated": "2024-04-12 07:13:03.339Z"
  },
  {
    "adresse": "30 Rue du Centre , Lyon 69000",
    "collectionId": "iiey60bvm8pv197",
    "collectionName": "maison",
    "created": "2024-04-12 07:15:02.473Z",
    "favori": true,
    "id": "h20wwhxywmn6t83",
    "image": "appart_ville_H2UO60e4vT.jpeg",
    "nbChambres": 2,
    "nbSdb": 1,
    "nomMaison": "Appartement en Ville ",
    "prix": 300000,
    "surface": 100,
    "updated": "2024-04-12 07:15:02.473Z"
  },
  {
    "adresse": "40 Route des Cimes , 74200",
    "collectionId": "iiey60bvm8pv197",
    "collectionName": "maison",
    "created": "2024-04-12 07:17:12.146Z",
    "favori": false,
    "id": "eyuhxojw1w6k3ug",
    "image": "nuit_dans_un_chalet_en_bois_pres_de_thonon_les_bains_dV3yw0Wvq5.jpeg",
    "nbChambres": 3,
    "nbSdb": 2,
    "nomMaison": "Chalet à la Montagne ",
    "prix": 600000,
    "surface": 200,
    "updated": "2024-04-12 07:17:12.146Z"
  },
  {
    "adresse": "50 Avenue des Arbres , Audincourt 25400",
    "collectionId": "iiey60bvm8pv197",
    "collectionName": "maison",
    "created": "2024-04-12 07:19:18.452Z",
    "favori": true,
    "id": "h02vdwjba2o2jw8",
    "image": "maison_banlieu_r0BWcqUkEY.jpeg",
    "nbChambres": 6,
    "nbSdb": 4,
    "nomMaison": "Maison Moderne en Banlieue",
    "prix": 850000,
    "surface": 400,
    "updated": "2024-04-12 07:19:18.452Z"
  }
]
</script>

<template>
  <div>
    <MaisonCard v-for="maison in maisonsListe" :key="maison.nom" v-bind="maison" />
    <h1 class="text-2xl">Bonjour monde !</h1>
  </div>
</template>
