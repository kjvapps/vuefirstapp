<template>
<section>
   <header><h2>My Friends</h2></header>
        <ul>
                <friend-contact
                v-for="friend in friends"
                :key="friend.id"
                :name="friend.name"
                :phone-number='friend.phone'
                :email-address='friend.email'
                :is-favorite="true" 
                ></friend-contact>
        </ul>
   </section>
</template>

<script>
export default {
    data() {
        return {
            friends: [{
                id: 'manuel',
                name: 'Manuel Lorenz',
                phone: '555-555',
                email: 'manuel@localhost.com'
            },
            {
                id: 'julie',
                name: 'Julue Jones',
                phone: '444-555',
                email: 'julie@localhost.com'
            }
            ]
        }
    },
    
}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Jost@display=swap')

</style>
