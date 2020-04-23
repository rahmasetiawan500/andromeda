<template>
    <div class="profile">

    <div class="container">
        <div class="row justify-content">
            <div class="col-lg-6">
            <div class="media text-left">
    <img src="../assets/logo.png" class="user-pic  mr-3" >
    <div class="media-body">
        <h5 class="mt-0"> {{ firstName }} JavaScript</h5>
        Hallo saya framework frontend
            </div>
    </div>
            </div>
        </div>
    </div>
    </div>
</template>

<script>

import 'bootstrap/dist/css/bootstrap.css'

export default {

    name: "Profile",

    data: function() {
        return {
            firstName: 'Vue'
        }
    },

    components: {

    }
};
</script>

<style scoped>

.user-pic{

    width: 80px;
    height: 80px;
}

</style>