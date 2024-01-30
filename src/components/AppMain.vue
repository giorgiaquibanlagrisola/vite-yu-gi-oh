<script>
export default {
    data() {
        return {

        };
    },
    props: {
        allCards: Array
    }
}
</script>

<template>
    <main>
        <div class="container">
            <div class="row">
                <form action="">
                    Alien
                </form>
            </div>
        </div>
        <div class="container">
            <div class="row d-flex justify-content-center">
                <div class="col-lg-2 col-md-6" v-for="(card, i) in allCards" 
                :key="i">
                    <div class="singleCard">
                        <div>
                            <img :src="card.image_url" :alt="card.name">
                        </div>
                        <div>
                            <h4 class="fs-6">
                                {{ card.name }}
                            </h4>
                            <h5 class="fs-6">
                                {{ card.archetype }}
                            </h5>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
</style>
