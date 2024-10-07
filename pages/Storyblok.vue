<template>
    <div class="p-6" v-if="data">
        <pre> {{ data }}</pre>
<h1></h1>
<p></p>
<img src="" alt=""/>
    </div>
</template>

<script setup>
import { ref, onMounted} from 'vue'
const data = ref(value, null)
onMounted(hook, async() => {
    data.value= await fetch(
        input,'https://api.storyblok.com/v2/cdn/stories/homepage?version=draft&token=p10LrVBkFDR5GY05E96h3Att').then((response) => response.json())

})

</script>