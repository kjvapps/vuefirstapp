<template>
<section>
   <header><h2>My Friends</h2></header>
        <ul>
            <li>
                <friend-contact
                name="Manuel Lorenz"
                phone-number='555-555'
                email-address='manuel@localhost.com'
                is-favorite='1'
                ></friend-contact>
                <friend-contact
                name="Julie Jones"
                phone-number='444-555'
                email-address='julie@localhost.com'
                ></friend-contact>
            </li>
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
