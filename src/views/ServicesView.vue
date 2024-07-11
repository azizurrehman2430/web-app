<template>
    <v-row class="mt-16">
      <v-col cols="12" md="4">
        <v-img src="../assets/And.jpg"></v-img>
        <v-card
          text="We specialize in Android app development that merges innovation with practicality, transforming your
                  concepts into functional solutions. Our team prioritizes user-friendly interfaces, ensuring seamless
                  navigation and captivating experiences."
          title="Andriod Development"
        ></v-card>
      </v-col>
  
      <v-col cols="12" md="4">
        <v-img src="../assets/mda.png"></v-img>
        <v-card>
          <template v-slot:title>
            UX/UI Design </template>
  
          <!-- <template v-slot:subtitle>
            This is a card subtitle
          </template> -->
  
          <template v-slot:text>
            "We craft intuitive user experiences and captivating interfaces that resonate. Our process focuses on
                  seamless interactions and stunning designs to elevate your digital presence, turning ideas into
                  engaging experiences.Our team prioritizes user-friendly interfaces, ensuring seamless
                  navigation and captivating experiences
                </template>
        </v-card>
        </v-col>
  
      <v-col cols="12" md="4">
        <v-img src="../assets/sd.webp"></v-img>
        <v-card>
          <v-card-item>
            <v-card-title>Software Development</v-card-title>
  
            <!-- <v-card-subtitle>This is a card subtitle</v-card-subtitle> -->
          </v-card-item>
  
          <v-card-text>
            We specialize in creating user-friendly websites that prioritize speed, security, and online
                  visibility. Our responsive designs enhance brand presence, driving engagement, and ensuring success
                  for your website by delivering a seamless user experience.Our team prioritizes user-friendly interfaces, ensuring seamless
                  navigation and captivating experiences.
                </v-card-text>
        </v-card>
        </v-col>
    </v-row>
  </template>
  <script>
  export default {
    name: 'services-us',
  };
</script>