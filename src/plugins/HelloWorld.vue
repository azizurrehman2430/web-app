<template>
  <v-container class="mt-16">
    <v-row class="text-center">
      <v-col cols="12">
        <v-img :src="require('../assets/aziz.png')" class="my-3" contain height="200" />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to the portfolio
        </h1>


        <p class="subheading font-weight-regular">
          I'm a web Designer with extensive experiencefor over 6 month.

          Expertise is to create a website,website design,Fronted design and programming.I am a skilled web designer
          with over 6month of experience in the industry.My plan lies in creating captivating website designe and
          implementing them through fronted development. I take pride in staying update with current design trends and
          leveraging my creativity to produce visually appealing & user-family websites.Throughout my career,I have
          developed a deep understanding of user experience(UX) and user interface(UI) principles.By putting myself in
          the shoes of end-users, I strive to create intutive and seamless browsing experiences. I beleive that a
          well-designed website should not only look visually appealing, also provide a smooth and enjoyable interaction
          for visitors. When starting a new project, I thoroughly research & analyze the target audience and the
          client's specific requirements.This enables me to tailor my design to meet their expactations and deliever a
          unique online presence that aligns with their brand identity.
          <br>
        </p>

        <div>
          <v-btn icon href="https://www.facebook.com/profile.php?id=100074228396400&mibextid=ZbWKwL" target="blank"
            class="mt-6 mr-4">
            <v-icon size="45" color="blue-darken-2">mdi-facebook</v-icon>
          </v-btn>
          <v-btn icon href="https://github.com/azizurrehman2430" target="blank" class="mt-6 mr-4">
            <v-icon size="45" center>mdi-github</v-icon>
          </v-btn>
          <v-btn icon href="https://www.linkedin.com/in/aziz-ur-rehman-637008247/" target="blank" class="mt-6 mr-4">
            <v-icon size="45" color="blue">mdi-linkedin</v-icon>
          </v-btn>
          <v-btn icon href="https://www.instagram.com/rai_aziz24?utm_source=qr&igsh=MW02YzVoc2JpbnExaQ== " target="_blank"
            class="mt-6 mr-4">
            <v-icon size="45" color="red">mdi-instagram</v-icon>
          </v-btn>
        </div>

        <v-btn class="mt-10" type="submit" color="success" v-on:click="logUserData()">
          Read more
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

export default {
  name: 'HelloWorld',

  data: () => ({
    ecosystem: [
      {
        text: 'vuetify-loader',
        href: 'https://github.com/vuetifyjs/vuetify-loader/tree/next',
      },
      {
        text: 'github',
        href: 'https://github.com/vuetifyjs/vuetify/tree/next',
      },
      {
        text: 'awesome-vuetify',
        href: 'https://github.com/vuetifyjs/awesome-vuetify',
      },
    ],
    importantLinks: [
      {
        text: 'Chat',
        href: 'https://community.vuetifyjs.com',
      },
      {
        text: 'Made with Vuetify',
        href: 'https://madewithvuejs.com/vuetify',
      },
      {
        text: 'Twitter',
        href: 'https://twitter.com/vuetifyjs',
      },
      {
        text: 'Articles',
        href: 'https://medium.com/vuetify',
      },
    ],
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com',
      },
      {
        text: 'Roadmap',
        href: 'https://vuetifyjs.com/introduction/roadmap/',
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }),
}
</script>