<template>
                                <div>
                                    <div class="form-check">
                                    <input class="form-check-input" onclick="" type="checkbox" value="" id="defaultCheck1">
                                    <label class="form-check-label item" v-bind:class="{'item-completed':tugasSaya.isDone}" for="defaultCheck1">
                                       {{ tugasSaya.nama }}
                                    </label>
                                </div>
</div>
</template>

<script>
    import 'bootstrap/dist/css/bootstrap.css';
    export default {
            name: "ItemTugas",
            props: ["tugasSaya"]
            };
</script>

<style scoped>
  
</style>