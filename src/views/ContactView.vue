<template>
    <v-app class="mt-16 mb-8">
      <v-main >
  
        <div class="mt-16">
          <v-sheet class="mx-auto" max-width="400">
            <span ><h1 class="text-center">Contact Us</h1></span>
            <v-form @submit.prevent ref="form">
              <v-text-field v-model="userData.name" class="text-black" label="Name" append-inner-icon="mdi-account"
                variant="outlined" color="blue" :counter="20" :rules="dataValidationRules.name" required>
              </v-text-field>
              <v-text-field v-model="userData.email" label="Email" append-inner-icon="mdi-email" variant="outlined"
                color="blue" hint="www.example@gmail.com" :rules="dataValidationRules.email"></v-text-field>
              <v-text-field v-model="userData.password" label="Password" append-inner-icon="mdi-eye" variant="outlined"
                color="blue"></v-text-field>
              <v-text-field v-model="userData.phNumber" label="Phone No" append-inner-icon="mdi-phone No" variant="outlined"
                color="blue" :rules="dataValidationRules.phone"></v-text-field>
              <v-textarea v-model="userData.address" label="Address" rows="2" clear-icon="mdi-close-circle" clearable
                append-inner-icon="mdi-home" variant="outlined" :rules="dataValidationRules.address" color="blue">
              </v-textarea>
      <v-checkbox type="checkbox" label="Add Bonus" v-on:click="AddBonus()">
    
      </v-checkbox>
      <div v-if="addBonus">
        <v-text-field  v-model="userData.bonus" label="Add Bonus Amount"  variant="outlined"
        color="blue">
        </v-text-field>
      </div>
              <v-btn class="mt-2" type="submit" color="success" block v-on:click="logUserData()">
                submit
              </v-btn>
              <v-btn class="mt-2" block v-on:click="clearForm()">
                Clear
              </v-btn>
              <br>
            </v-form>
          </v-sheet>
        </div>
      </v-main>
    </v-app>
    </template>
    <script>
    export default {
      name: 'contact-us',
      data() {
        return {
        addBonus:false,
          userData: {
            name: '',
            email: '',
            password: '',
            phNumber: '',
            address: '',
            bonus:0
          },
    
          dataValidationRules: {
            name: [
              value => {
                if (value) return true
                return 'You must enter a Name.'
              },
            ],
            phone: [
              value => {
                if (value?.length > 9 && /[0-9-]+/.test(value)) return true
    
                return 'Phone number needs to be at least 9 digits.'
              },],
            email: [
              value => {
                if (/^[a-z.-]+@[a-z.-]+\.[a-z]+$/i.test(value)) return true
    
                return 'Must be a valid e-mail.'
              },],
    
            address: [
              value => {
                if (value?.length > 25) return true
                return 'Address must be at least 25 characters.'
              }
            ]
          }
        }
    
      },
      methods: {
        logUserData() {
          console.log(this.userData);
        },
        clearForm(){
          this.userData.name='';
          this.userData.address='';
          this.userData.email='';
          this.userData.password='';
          this.userData.phNumber='';
          this.reset();
          },
          reset () {
            this.$refs.form.reset()
          },  
          AddBonus(){
            this.addBonus= !this.addBonus;
          }    
      }
    }
    
    
    </script>