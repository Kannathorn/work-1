<template>
  <v-container fluid class="pa-0">
    <v-row align="center">
      <v-col cols="12" sm="6">
        <div class="text-center">
          <div class="my-2">
            <nuxt-link to="/fing">
              <v-btn color="secondary" dark>กิจกรรมหน้าเสาธง</v-btn>
            </nuxt-link>
          </div>
          <div class="my-2">
            <nuxt-link to="/homeroom">
              <v-btn color="primary" dark>กิจกรรมโฮมรูม</v-btn>
            </nuxt-link>
          </div>
          <div class="my-2">
            <nuxt-link to="/special">
              <v-btn color="warning" dark>กิจกรรมพิเศษ</v-btn>
            </nuxt-link>
          </div>
         <div class="my-2">
            <nuxt-link to="/ex01">
              <v-btn color="warning" dark>หน้าประวัติ</v-btn>
            </nuxt-link>
          </div>
           <div class="my-2">
            <div><button @click="doindex">HOME</button></div>
          </div>
          
        </div>
      </v-col>
      <v-col cols="12" sm="6">
        <div class="text-center">
          <div class="my-2">
            <v-btn color="secondary" fab x-small dark>
              <v-icon>mdi-television</v-icon>
            </v-btn>
          </div>
          <div class="my-2">
            <v-btn color="primary" fab small dark>
              <v-icon>mdi-pencil</v-icon>
            </v-btn>
          </div>
          <div class="my-2">
            <v-btn color="warning" fab dark>
              <v-icon>mdi-account-circle</v-icon>
            </v-btn>
          </div>
          <div class="my-2">
            <v-btn color="error" fab large dark>
              <v-icon>mdi-alarm</v-icon>
            </v-btn>
          </div>
          <div class="my-2">
            <v-btn color="success" fab x-large dark>
              <v-icon>mdi-domain</v-icon>
            </v-btn>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      name: "Kannathorn",
      age: 19,
    }
  },
  methods:{
    doex01(){
    this.$router.push('/ex01')
    },
    },
     methods:{
    doindex(){
    this.$router.push('/')
    },
  },
}
</script>