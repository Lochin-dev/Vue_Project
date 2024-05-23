<template>
    <div class="container">
        <div class="d-flex flex-column flex-md-row align-items-center py-2 mb-3 border-bottom">
            <a class="d-flex align-items-center link-body-emphasis text-decoration-none gap-2">
                <img :src="logo" alt="logo" class="w-25" style="cursor:pointer " @click="toHomeHandler">
                <!-- <p class="m-0">Lochin Dev</p> -->
            </a>

            <nav class="d-inline-flex mt-2 mt-md-0 ms-md-auto">
                <a>
                    <RouterLink class="me-3 py-2 link-body-emphasis text-decoration-none" :to="{ name: 'login' }">
                        Login
                    </RouterLink>
                </a>
                <a>
                    <RouterLink class="py-2 link-body-emphasis text-decoration-none" :to="{ name: 'register' }">
                        Register
                    </RouterLink>
                </a>
            </nav>
        </div>
    </div>
</template>
<script>
import { logo } from "../constants"
export default {
    data() {
        return { logo }
    },
    methods: {
        toHomeHandler() {
            return this.$router.push("/")
        }
    }
}
</script>
<style></style>