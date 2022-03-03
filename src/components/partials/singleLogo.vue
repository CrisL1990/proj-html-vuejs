<template>
    <section>
        <div>
            <img :src="logo" alt="Company Logo">
        </div>
    </section>
</template>

<script>
export default {

    name: 'sngleLogo',

    props:{
        'logo': String,
    }
}
</script>

<style scoped lang="scss">

</style>