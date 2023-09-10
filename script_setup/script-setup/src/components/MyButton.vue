<template>
    <button>{{ text }}</button>
</template>



<!-- old way -->
<!-- <script>
    export default {
        props: {
            text: {
                type: String,
                default: 'No text specified'
            }
        }
    }
</script> -->

<script setup>

const props = defineProps({
    text: {
        type: String,
        default: "no text specified"
    }
});

</script>