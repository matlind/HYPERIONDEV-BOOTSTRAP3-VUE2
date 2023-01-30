<template>
    <div class="coding-journey container">
        <div class="col-xs-9">
            <div class="row">
                <div class="col-xs-12">
                    <h3> {{ title }}</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-xs-9">
                    {{ stats.label }}
                </div>
            </div>
            <div class="row">
                <div class="col-xs-9">
                    {{ stats.label2 }}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "CodingJourney",
    data() {
        return {
            title: 'Your coding journey',
            stats: {
                label: "Total programs written",
                label2: "Total code reviews"
            }
        }
    }
}
</script>

<!-- <style>
.CardMedia__button {
    list-style-type: none;
}
</style> -->