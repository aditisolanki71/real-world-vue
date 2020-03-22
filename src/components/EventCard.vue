<template>
    <div>
         <router-link :to="{name: 'event-show',params: {id : '1'}}">Show event #1
        <span>@{{event.time}} on {{event.name}}</span>
        <h1>
          {{event.title}}
        </h1>
        <span>{{event.attendiee.length}} attending </span>
        </router-link>
    </div>
</template>

<script>
export default {
    data() {
        return {
            event: {
                id: '1',
                title: 'aditi',
                date: 'sunday 22 mar 2020',
                time: '8pm',
                attendiee: [ 
                    {id: '1' , name: 'moni'},
                    {id: '2' , name: 'monika'}
                ]
            }
    }
}
}
</script>
<style scoped>
h4 {
    color: green
}
</style>
