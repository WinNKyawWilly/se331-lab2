<script setup lang="ts">
import { ref } from 'vue'
import Event from '@/types/Event'

defineProps<{
    event: Event
}>()
</script>

<template>
    <div class="organizer-info"> 
        <div class="event-card">
            <h2>{{ event.organzier}}</h2>
            <h2>{{ event.category}}</h2>
        </div>
    </div>
</template>

<style scoped>
.organizer-info .event-card {
    padding: 20px;
    width: 250px;
    cursor: pointer;
    border: 1px solid #39495c;
    margin-bottom: 18px
}

.organizer-info .event-card:hover {
    transform: scale(1.05);
    box-shadow: 0 3 12px rgba(0, 0, 0, 0.2);
}

.organizer-info .event-card h2 {
    margin: 0;
    font-size: 1.5rem;
    color: #39495c;
}
</style>