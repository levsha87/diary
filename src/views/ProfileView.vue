<template>
    <div>
        <h1>Profile View</h1>
        <StudentProfile />
    </div>
</template>

<script>
import StudentProfile from '@/components/StudentProfile.vue';

export default {
    name: 'ProfileView',
    components: {
        StudentProfile
    },
}
</script>

<style scoped>
</style>