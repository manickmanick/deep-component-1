<template>
    <div>

        <h2>Manage Goals</h2>
        <input type="text" ref="goal">
        <button @click="setGoal">Set Goal</button>
    </div>
</template>


<script>
export default {
    methods: {
        setGoal ()
        {
            const enteredValue = this.$refs.goal
            if (enteredValue === "")
            {
                alert("type something")
            }
        }
    }
}
</script>