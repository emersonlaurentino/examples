<template>
    <div class="container" style="padding: 50px 0 100px 0">
        <Account v-if="user" />
        <Auth v-else />
    </div>
</template>

<script setup>
const user = useUser();
user.value = useSupabaseUser()
</script>
