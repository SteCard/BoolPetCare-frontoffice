<!-- JAVASCRIPT & VUE.JS -->
<script>
import axios from 'axios';

export default {

    components: {
        //
    },

    data() {
        return {
            baseUrl: 'http://localhost:8000',
            loading: true,
            // animals: [],
        }
    },

    created() {
        this.getProjects();
    },

    methods: {
        getProjects() {

            this.loading = true;

            // axios.get(`${this.baseUrl}/api/projects`).then((response) => {
            //     if (response.data.success) {

            //         this.projects = response.data.results;

            //         // console.log(response.data.results)

            //         this.loading = false;
            //     }
            // })
        },
    },
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <div class="container pb-5">
        <div class="row justify-content-center">
            <div class="col-12 py-5">
                <h1 class="text-center">VITE PetCare</h1>
            </div>
            <!-- APP LOADER -->
            <!-- <div class="col-12 d-flex justify-content-center align-items-center py-5" v-if="loading">
                <AppLoader/>
            </div> -->
            <!-- IMG VIA API -->
            <!-- <div class="col-4 my-4"  v-for="project in projects" :key="project.id">
                <div class="card h-100">
                    <img class="card-img-top img-fluid" :src="`${baseUrl}/storage/${project.cover_image}`" :alt="`${project.title}-image`">
                    <div class="card-body h-50">
                        <h5 class="card-title py-2" v-text="project.title"></h5>
                        <p class="card-text py-2" v-text="project.description"></p>
                    </div>
                    <div class="card-footer text-center">
                        <a href="#" class="btn btn-primary">Visualizza Progetto</a>
                    </div>
                </div>
            </div> -->
        </div>
    </div>
</template>

<!-- STYLE SCSS -->
<style lang="scss">
// IMPORTO GENERALS.SCSS
@use '../styles/generals.scss' as *;
</style>