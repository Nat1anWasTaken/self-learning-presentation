<template>
  <vue-qrcode
    value="https://github.com/Nat1anWasTaken/self-learning-presentation"
    @change="onDataUrlChange"
  />
</template>
<script>
import VueQrcode from 'vue-qrcode'

export default {
  data() {
    return {
      dataUrl: null,
    }
  },
  components: {
    VueQrcode,
  },
  methods: {
    onDataUrlChange(dataUrl) {
      this.dataUrl = dataUrl
    },
  },
}
</script>