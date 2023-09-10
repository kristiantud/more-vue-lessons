<template>
    <h1 @click="handleHeadingClick">My name is {{name}}, I am {{age}} years old.</h1>
    <MyButton text="My Button Text"/>
</template>

<script setup>
    import { ref } from 'vue';
    import MyButton from "@/components/MyButton.vue"
    // old way to add component: 
    // import MyButton from @/components/MyButton.vue
    // after setup():
    // components: { MyButton }

    const name = ref('Bob');
    const age = ref(75);

    // this way, we no longer need the return statement
    const handleHeadingClick = () => {
        name.value = 'Steven';
        age.value = 29;
    }


</script>