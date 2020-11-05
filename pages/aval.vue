<template>
    <main>
        <!--? Hero Start -->
        <div class="slider-area2">
            <div class="slider-height2 d-flex align-items-center">
                <div class="container">
                    <div class="row">
                        <div class="col-xl-12">
                            <div class="hero-cap text-center">
                                <h2>Aval</h2>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Hero End -->
        <!--? Brand Area Start -->
        <section class="team-area pb-100">
            <div class="container">
                <div class="row">
                    <div class="col-md-8 offset-md-2">
                        <div class="card mt-5">
                            <div class="card-body">
                                <p>12 puntos</p>
                                <ul>
                                    <li>Consejo Mexicano de
Ginecología y Obstetricia, A.C.</li>
                                </ul>
                                <br>
                                <p>12 puntos</p>
                                <ul>
                                    <li>Consejo Mexicano de Oncología</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Brand Area End -->
    </main>
</template>

<script>
  import OrganizerComponent from "../components/OrganizerComponent";

  export default {
    components: {OrganizerComponent},
    data() {
      return {
        organizers: [],
        groups: [],
      }
    },
    async mounted() {
      this.organizers = await this.$axios.$get('/board-directors?board_director_category_null=true');
      this.groups = await this.$axios.$get('/board-director-categories');
    }
  }
</script>

<style lang="scss" scoped>
    .slider-area2 {
        background-image: url(/images/cover_main.jpg);
    }
    li {
        list-style: circle !important;
        margin-left: 20px;
    }
</style>
