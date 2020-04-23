<template>
    <div class="project">
        <div class="container">
            <div class="row header mb-5 p-3">
                <div class="col-lg-12">
                    <h3>what i do?</h3>
                </div>
            </div>
            <div class="container">
                <div class="row content">
                    <div class="col-lg-12">
                        <div class="pekerjaan-rumah">
                            <div class="row">
                                <div v-for="tugasSaya in tugas" v-bind:key="tugasSaya.id" class="mb-3 tugas col-lg-12 text-left">
                                    <ItemTugas v-bind:tugasSaya="tugasSaya" />
                            </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import 'bootstrap/dist/css/bootstrap.css';
    import ItemTugas from '../components/ItemTugas';

    export default {

        name: "Project",

        data: function () {
            return {
                tugas: [{
                        id: 1,
                        nama: "Ngoding Berkah",
                        isDone: false
                    },
                    {
                        id: 2,
                        nama: "Puasa Berkah",
                        isDone: false
                    },
                    {
                        id: 3,
                        nama: "Ibadah Berkah",
                        isDone: false
                    },
                    {
                        id: 4,
                        nama: "Dapat Hadiah",
                        isDone: false
                    }
                ]
            }
        },

        components: {
            ItemTugas
        }
    };
</script>

<style scoped>
    .header {
        background: #1abc9c;
    }

    .header h2 {

        margin: 0;

    }
    .tugas .item {
        font-size:20px;

    }
        .item-completed {
        color: #1abc9c;
    }
</style>