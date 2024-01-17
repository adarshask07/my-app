<template lang="en-us">
    <div class="bg-white w-11/12 rounded-lg shadow-lg p-4 text-center flex justify-around">
        
        <h2 v-for="(Student, index) in Students" :key='Student.roll_no' class="text-3xl font-bold mb-2 mt-3">
                {{ Student.name }} - Key: {{ index }}
        </h2>

        <slot></slot>
  </div>
</template>
<script>
export default {
    name: "MainComponent",
    data() {
        return {
            Students: [
                {
                    name: "Adarsh",
                    roll_no: 25
                },
                {
                    name: "Shravan",
                    roll_no: 25
                },
                {
                    name: "Yash",
                    roll_no: 36
                }
            ]
        }
    }

}
</script>
<style lang="">
    
</style>