<template>
<div>
    <table border="1px">
    <thead><tr><th>Name</th><th>address</th><th>City</th></tr></thead>
    <tbody>
    <tr  v-for="items in student" :key="items"><td>{{items.sname}}</td> <td>{{items.address}}</td><td>{{items.city}}</td></tr>
    </tbody></table>
    <table border="1px">
    <thead><tr><th>Name</th><th>address</th><th>City</th></tr></thead>
    <tbody>
    <tr  v-for="items of student" :key="items"><td>{{items.sname}}</td> <td>{{items.address}}</td><td>{{items.city}}</td></tr>
    </tbody></table>
</div>
</template>
<script >
export default {
    name:'FooLoop',
    data() {
        return {
            student:[{sname:'swapnil',address:'pune',city:'pune'},
            {sname:'madhuri',address:'pune',city:'pune'},
            {sname:'kunal',address:'solapur',city:'solapur'},]
        }
    },

}
</script>