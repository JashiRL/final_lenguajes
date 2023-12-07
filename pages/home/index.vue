<script >
import homeVue from '~/components/Users/home.vue'
export default {

    layout: 'dashboard',
    components: {
        homeVue
    },

   
    mounted() {
    const datoemail = sessionStorage.getItem('email')
    if (!datoemail ) {
        this.$router.push("/")
    }
        }
}

</script>

<template>
     <div class="ma-1">
        <homeVue />
    </div>
</template>

<style  scoped>

</style>