<template>
<h1>Dynamic content</h1>
<button v-on:click="tab='java'">load java</button>
<button v-on:click="tab='php'">load php</button>
<button v-on:click="tab='node'">load node</button>
<component :is="tab" />
</template>

    
<script>
import java from './java.vue';
import php from './php.vue';
import node from './node.vue';
export default {
    name: 'Home',
    components: {
        java,
        php,
        node
    },
    data() {
        return {
            tab: 'node'
        }
    }

}
</script>
