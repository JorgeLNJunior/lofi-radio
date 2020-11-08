<template>
  <v-container fluid class="fill-height">
    <v-row align="center" justify="center">
      <v-col cols="md-8">
        <v-card>
          <v-card-text>
            <aplayer autoplay
              :list="music"
              :music="music[0]"
              theme="#42A5F5"
              :listFolded="true"
              controls
            />
            <v-row justify="start">
              <v-col cols="6">
                <div>
                  <b>Playlist: </b>
                  <span>Default</span>
                </div>
                <div>
                  <b>Author: </b>
                  <span>Lo-Fi Radio</span>
                </div>
                <div>
                  <b>URL: </b>
                  <span>???</span>
                </div>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

import aplayer from 'vue-aplayer'

export default {
  name: 'Home',
  components: {
    aplayer
  },
  data: () => ({
    music: [{
      title: 'Call me',
      artist: '90sFlav',
      src: 'https://lofiradio.blob.core.windows.net/musics/90s_Flav_-_Call_me.mp3',
      pic: 'https://lastfm.freetls.fastly.net/i/u/ar0/4a5d15046b204ba75d092fb9d013ae6c.jpg'
    },
    {
      title: 'Proud of You',
      artist: 'A L E X',
      src: 'https://lofiradio.blob.core.windows.net/musics/A_L_E_X_-_Proud_of_You_(feat._Alicks).mp3',
      pic: 'https://m.media-amazon.com/images/I/81uvz8J86JL._SS500_.jpg'
    },
    {
      title: 'Golden Mercedes',
      artist: 'A L E X',
      src: 'https://lofiradio.blob.core.windows.net/musics/A_L_E_X_-_Golden_Mercedes.mp3',
      pic: 'https://m.media-amazon.com/images/I/81uvz8J86JL._SS500_.jpg'
    },
    {
      title: 'The Burn Marks on My Epiano Wont Go Away',
      artist: 'A L E X',
      src: 'https://lofiradio.blob.core.windows.net/musics/A_L_E_X_-_The_Burn_Marks_on_My_Epiano_Wont Go_Away.mp3',
      pic: 'https://m.media-amazon.com/images/I/81uvz8J86JL._SS500_.jpg'
    },
    {
      title: 'Espresso',
      artist: 'Aso',
      src: 'https://lofiradio.blob.core.windows.net/musics/Aso_-_Espresso.mp3',
      pic: 'https://i.ytimg.com/vi/mlxO2cJIMKw/maxresdefault.jpg'
    },
    {
      title: 'Drowsy',
      artist: 'brillion',
      src: 'https://lofiradio.blob.core.windows.net/musics/brillion_-_Drowsy.mp3',
      pic: 'https://images.shazam.com/coverart/t510917073-b1503517553_s400.jpg'
    },
    {
      title: 'sunday morning bacon',
      artist: 'Delayde',
      src: 'https://lofiradio.blob.core.windows.net/musics/Delayde_-_sunday_morning_bacon.mp3',
      pic: 'https://i1.sndcdn.com/artworks-000473886630-09suce-t500x500.jpg'
    },
    {
      title: 'Seaside',
      artist: 'DLJ & S-Ilo',
      src: 'https://lofiradio.blob.core.windows.net/musics/DLJ_&_S-Ilo_-_Seaside.mp3',
      pic: 'https://i1.sndcdn.com/artworks-000402447321-mrq8ea-t500x500.jpg'
    },
    {
      title: 'Carried Away',
      artist: 'goosetaf, The Field Tapes, Francis',
      src: 'https://lofiradio.blob.core.windows.net/musics/goosetaf,_The_Field_Tapes,_Francis_-_Carried_Away.mp3',
      pic: 'https://i.ytimg.com/vi/mlxO2cJIMKw/maxresdefault.jpg'
    },
    {
      title: 'monster gambling in tokyo',
      artist: 'Idealism',
      src: 'https://lofiradio.blob.core.windows.net/musics/Idealism_-_monster_gambling_in_tokyo.mp3',
      pic: 'https://m.media-amazon.com/images/I/91tI2pKob2L._SS500_.jpg'
    },
    {
      title: 'Snow & Sand',
      artist: "j' san, Epektase",
      src: "https://lofiradio.blob.core.windows.net/musics/j'san,_Epektase_-_Snow_Sand.mp3",
      pic: 'https://images.shazam.com/coverart/t503860875-b1489080371_s400.jpg'
    },
    {
      title: 'cozy winter',
      artist: "j'san",
      src: "https://lofiradio.blob.core.windows.net/musics/j'san_-_cozy_winter.mp3",
      pic: 'https://f4.bcbits.com/img/a1035755920_10.jpg'
    },
    {
      title: 'beingwithu',
      artist: 'Kudasaibeats, Luv.Ly',
      src: 'https://lofiradio.blob.core.windows.net/musics/Kudasaibeats,_Luv.Ly_-_beingwithu.mp3',
      pic: 'https://images.genius.com/4181347b736f69b428a2ae14110e266c.1000x1000x1.jpg'
    },
    {
      title: 'Lunar Drive',
      artist: 'Mondo Loops',
      src: 'https://lofiradio.blob.core.windows.net/musics/Mondo_Loops_-_Lunar_Drive.mp3',
      pic: 'https://images.shazam.com/coverart/t503860875-b1489080371_s400.jpg'
    },
    {
      title: 'Eternal Youth',
      artist: 'Rude',
      src: 'https://lofiradio.blob.core.windows.net/musics/Rude_-_Eternal_Youth.mp3',
      pic: 'https://i.ytimg.com/vi/YAtdukYmnb0/maxresdefault.jpg'
    },
    {
      title: 'Snowman',
      artist: 'Wys',
      src: 'https://lofiradio.blob.core.windows.net/musics/Wys_-_Snowman.mp3',
      pic: 'https://images.shazam.com/coverart/t503860875-b1489080371_s400.jpg'
    }]
  })
}
</script>

<style>

</style>
