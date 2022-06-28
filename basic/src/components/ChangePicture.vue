<template>
    <div>
        <button @click="$emit('changePicture')">Change Picture</button>
    </div>    
</template>

<script>
    export default {
        name: 'ChangePicture',
        emits: ['changePicture']
    }
</script>