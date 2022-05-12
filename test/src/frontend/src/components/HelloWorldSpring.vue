<template>
    <div class="hello">
        <h1>{{ items.msg }}</h1>
    </div>
</template>

<script lang="ts">
import axios from 'axios';

export default {
    items!: String,
    name: 'HelloWorldSpring',
    props: {
        data: String
    },
    methods: {
        func() {
        }
    },
    created() {
        axios.get("/api/hello")
            .then(res => {
                console.log(res.data);
                this.items = res.data
            })
            .catch(err => {
                console.log(err);
            });
    },
    data() {
        return {
            items: [],
        };
    },
}
</script>