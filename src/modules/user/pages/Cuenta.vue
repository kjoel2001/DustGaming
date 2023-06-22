<template>
    <main class="main">
      <div class="account">
        <div class="container">
          <h1 class="account__title">Información de la cuenta</h1>
          <div class="account__form">
            <form @submit.prevent="changeAccount">
              <p><strong>Correo electrónico:</strong> {{ email }}</p>
              <br> <!-- Espacio agregado -->
              <input v-model="newEmail" type="text" class="txt txt--left" placeholder="Nuevo correo electrónico" />
              <button type="button" class="btn btn--brand btn--boxshadow w--100" @click="changeEmail">Cambiar correo electrónico</button>
              <br>
              <input v-model="newPassword" type="password" class="txt txt--left" placeholder="Nueva contraseña" />
              <button type="button" class="btn btn--brand btn--boxshadow w--100" @click="changePassword">Cambiar contraseña</button>
              <br>
            </form>
          </div>
        </div>
      </div>
    </main>
  </template>
  
  
  <script>
  import { auth } from '@/firebase.js'
  
  export default {
    data() {
      return {
        email: '',
        username: '',
        newPassword: '',
        newEmail: ''
      }
    },
    mounted() {
      const currentUser = auth.currentUser
      if (currentUser) {
        this.email = currentUser.email
        this.username = currentUser.displayName
      }
    },
    methods: {
      async changePassword() {
        try {
          await auth.currentUser.updatePassword(this.newPassword)
          alert('La contraseña se ha cambiado exitosamente')
          this.newPassword = ''
        } catch (error) {
          alert('Ha ocurrido un error al cambiar la contraseña: ' + error.message)
        }
      },
      async changeEmail() {
        try {
          await auth.currentUser.updateEmail(this.newEmail)
          alert('El correo electrónico se ha cambiado exitosamente')
          this.email = this.newEmail
          this.newEmail = ''
        } catch (error) {
          alert('Ha ocurrido un error al cambiar el correo electrónico: ' + error.message)
        }
      },
      changeAccount() {
        // Aquí puedes agregar cualquier lógica adicional relacionada con la cuenta
      }
    }
  }
  </script>
  
  <style>
  </style>
  