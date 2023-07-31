<template>
    <ul>
        <li v-for="goal in goals" :key="goal">
            <slot :item="goal" another-prop="xyz"></slot>
        </li>
    </ul>
</template>


<script>
export default {
    data ()
    {
        return {
            goals: ["finish course", "learn vue"]
        }
    }
}
</script>