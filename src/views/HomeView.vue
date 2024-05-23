<template>
    <div>
        <h1>Home {{ counter }}</h1>
        <div class="w-25">
            <Button @click="incrementHandler">Increment</Button>
        </div>

        <div class="w-25">
            <Button @click="decrementHandler">Decrement</Button>
        </div>
    </div>
</template>
<script>
export default {
    methods: {
        incrementHandler() {
            this.$store.commit('increment')
        },
        decrementHandler() {
            this.$store.commit('decrement')
        }
    },
    computed: {
        counter() {
            return this.$store.state.count
        }
    }
}
</script>
<style></style>