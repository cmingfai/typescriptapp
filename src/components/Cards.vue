<script lang="ts">

</script>

<script setup lang="ts">
import {GENDER, type Invitee} from "../types"

defineProps<{
    invitee: Invitee
}>()

</script>
<template>
    <div :style="{backgroundColor: invitee.gender===GENDER.MALE?'rgb(0,128,128)':'rgb(111,18,8)'}">
        {{invitee.name}}
    </div>
</template>

<style scoped>
div {
    background-color: aqua;
    border-radius: 5px;
    margin-top: 5px;
    text-align: center;
    padding: 3px;
    color: white;
}

</style>