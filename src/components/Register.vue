<template>
    <div class="text-center d-flex justify-content-center">
        <main class="form-signin w-25 m-auto mt-5">
            <form>
                <img :src="logo" alt="logo" class="w-50" style="cursor:pointer " @click="toHomeHandler">
                <h1 class="h3 mb-3 fw-normal mt-3">Register</h1>

                <Input :label="'Name'" :type="'text'" :placeholder="'Enter name'" />

                <Input :label="'Email address'" :type="'email'" :placeholder="'name@example.com'" />

                <Input :label="'Password'" :type="'password'" :placeholder="'Password'" />

                <Button type="submit">Register</Button>
                <!-- <button class="w-100 btn btn- btn-primary mt-3" type="submit">Sign in</button> -->
            </form>
        </main>
    </div>
</template>

<script>
import { logo } from "../constants"
export default {
    data() {
        return { logo }
    },
}
</script>
<style></style>