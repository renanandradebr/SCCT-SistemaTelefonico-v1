<template>
  <v-container>
    <div>
      <v-breadcrumbs divider="\">Dashboard \</v-breadcrumbs>
    </div>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img :src="require('../assets/logo-scct.png')" class="my-8 " contain height="100" />
      </v-col>

    </v-row>
    <v-divider></v-divider>
    <v-row>
      <v-col cols="12">
        <v-carousel class=" my-4" hide-delimiters>
          <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src"></v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>

    <v-divider></v-divider>


    <v-row class="buttons">
      <v-col cols="6" class="pa-md-4 mx-auto my-4">
        <v-card width="350" height="400" class="justify-center">

          <v-btn class="px-7 mx-10" color="blue" elevation="1" outlined>CADASTRO DE USUÁRIO</v-btn> <v-spacer></v-spacer>

          <v-btn class="px-14 my-4" color="blue" elevation="1" outlined>TELEFONE FIXO</v-btn><v-spacer></v-spacer>

          <v-btn class="px-10 my-auto" color="blue" elevation="1" outlined>TELEFONE CELULAR</v-btn><v-spacer></v-spacer>

          <v-btn class="px-8 my-4 my-2" color="blue" elevation="1" outlined>AGENDA TELEFÔNICA</v-btn>
          <v-btn class="px-9 my-auto" color="blue" elevation="1" outlined>SOLICITAR BACKUPS</v-btn>
          <v-btn class="my-4 my-2" color="blue" elevation="1" outlined>ACESSAR LOGS DE USUÁRIO</v-btn>
        </v-card>
      </v-col>
      <v-col cols="6" class="pa-md-4 mx-auto my-4">


      </v-col>
    </v-row>
    <v-row>
      <v-col>

      </v-col>
    </v-row>
  </v-container>
</template>



<script lang="ts">
export default {
  data() {
    return {
      items: [
        {
          src: 'https://images.pexels.com/photos/33999/pexels-photo.jpg',
        },
        {
          src: 'https://images.pexels.com/photos/13649371/pexels-photo-13649371.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
        },
        {
          src: 'https://images.pexels.com/photos/14038572/pexels-photo-14038572.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
        },
        {
          src: 'https://images.pexels.com/photos/821754/pexels-photo-821754.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
        },
      ],

    }
  },
}
</script>
