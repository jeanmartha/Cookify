<script setup>



</script>

<template>
  <v-responsive>
    <v-app :theme="theme">
      <!-- App Bar -->
      <v-app-bar class="px-3" elevation="3">
        <span class="text-h6 font-weight-medium">CooKify</span>
      </v-app-bar>

      <!-- Main Content -->
      <v-main>
        <v-container>
          <slot name="content"></slot>
        </v-container>
      </v-main>

      <!-- Footer -->
      <v-footer
      
        border
        app
        elevation="24"
        class="mx-auto font-weight-bold"
        :class="[theme === 'light' ? 'bg-surface-light' : 'bg-surface-dark']"
      >
        <span>© 2024 CooKify. All rights reserved.</span>
      </v-footer>
    </v-app>
  </v-responsive>
</template>
