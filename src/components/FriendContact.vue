<template>
    <li>
        <h2>{{ friend.name }}</h2>
        <button @click="toggleDetals">Show Details</button>
        <ul v-if="detailsAreVisible">
            <li><strong>Phone:</strong> {{ friend.phone}}</li>
            <li><strong>Email:</strong>{{ friend.email}}</li>
        </ul>
    </li>
</template>

<script>

export default{
    data() {
        return {
            detailsAreVisible: false,
            friend: { id: 'manuel',
                name: 'Manuel Lorenz',
                phone: '555-555',
                email: 'manuel@localhost.com'}
        }
    },
methods: {
    toggleDetals() {
        this.detailsAreVisible = !this.detailsAreVisible;
    }
}
}
   
</script>
