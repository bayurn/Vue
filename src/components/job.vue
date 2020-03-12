<template>
  <div>
    <b-col>
      <b-card
        :title="name"
        img-src="https://picsum.photos/300/200"
        img-alt="Ini foto bung!"
        style="max-width:20rem"
        class="mb-2"
        footer="Muehehehehe"
        footer-tag="footer"
      >
        <b-card-text>Anda tau siapa saya? Saya makhluk Mars!!</b-card-text>
        <b-button variant="primary">Apply</b-button>
      </b-card>
    </b-col>
  </div>
</template>

<script>
export default {
  props: ["name"]
};
</script>

<style lang="scss" scoped></style>
