<script>

// Importare componenti
import ShopLink from './ShopLink.vue';
import SponsorLinks from './SponsorLinks.vue';
export default {
    name: 'ShopSection',
    components: { ShopLink, SponsorLinks }
}
</script>

<template>
    <ShopLink />
    <SponsorLinks />
</template>

<style lang="scss" scoped></style>
