<template>
<v-container>
    <div v-bind:key="image.id" v-for="image in images">
        <h1>holi {{image.text}}</h1>
    </div>
    <h1>holi</h1>
     <v-btn small color="primary" v-on:click="print()">Primary</v-btn>

</v-container>
</template>

<script>
export default {
    name: 'ImageList',
    props:["images"],
    methods:{
        print() {
            console.log(this.images)
        }
    }
}

</script>