<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-white text-black">
      <q-toolbar>
        <q-avatar size="100px" class="q-ml-md">
          <img src="../assets/DekaBank_Deutsche_Girozentrale_201x_logo.svg" width="10%">
        </q-avatar>
        <q-toolbar-title class="text-weight-bold q-ml-md">
        NFT-Donation-Club
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>

export default ({
  name: 'MainLayout',

})
</script>
