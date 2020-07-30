<template>

    <v-form v-model="valid">
        <v-text-field v-model="userInfo.name"
            label="Name"
            :rules="[required('name'), minLength('name', 3)]" />

        <v-text-field v-model="userInfo.password"
            label="Password"
            :type="showPassword ? 'text' : 'password'"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
            counter:true
            :rules="[required('password'), minLength('password', 4)]" />

        <v-btn @click="submitForm(userInfo)" :disabled="!valid" href="/videos">{{ buttonText }}</v-btn>
    </v-form>
</template>

<script>
    import validations from "@/validations/validations";
    export default {
        data() {
            return {
                valid: true,
                showPassword: false,
                userInfo: {
                    name: '',
                    password: '',

                },
                ...validations
            }
        },
        props: ["submitForm", "buttonText", "hasName"]

    }
</script>

<style scoped lang="scss">


.v-form label, .label {
  font-size:1.75rem;
}
</style>
