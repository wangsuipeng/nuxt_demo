<template>
    <div>
        <h2>News-Content[{{$route.params.id}}]</h2>
        <nuxt/>
        <ul>
            <li>
                <!-- <a href="/">Home</a> -->
                <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    validate({ params }) {
        // Must be a number
        return /^\d+$/.test(params.id);
    },
    data() {
        return {
            title: this.$route.params.title,
        }
    },
    head() {
        return {
            title: this.title,
            meta: [
                {hid: 'description',name: 'news',content: 'This is news page'}
            ]
        }
    }
};
</script>
