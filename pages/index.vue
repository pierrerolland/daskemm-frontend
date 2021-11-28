<template>
  <v-row justify="center" align="center">
    <v-col>
      <regular-shirt :primary="primary" :secondary="secondary" :tertiary="tertiary" />
    </v-col>
    <v-col cols="4">
      <color-picker title="Primary color" v-model="primary" />
      <color-picker title="Secondary color" v-model="secondary" />
      <color-picker title="Tertiary color" v-model="tertiary" />
    </v-col>
  </v-row>
</template>

<script lang="ts">
import RegularShirt from '~/components/shirts/RegularShirt.vue';
import ColorPicker from '~/components/ColorPicker.vue';

export default {
  components: { RegularShirt, ColorPicker },
  data: () => ({
    primary: '#FFFFFF',
    secondary: '#333333',
    tertiary: '#FF5555'
  })
}
</script>
