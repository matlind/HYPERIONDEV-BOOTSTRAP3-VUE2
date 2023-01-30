<template>
    <div class="get-upgarde container">
        <div class="col-xs-9">
            <div class="row">
                <div class="col-xs-12">
                    <h3> {{ title }}</h3>
                </div>
            </div>
            <div class="col-xs-9">
                <div class="row">
                    <div class="col-xs-12">
                        <p> {{ text }}</p>
                    </div>
                </div>
                <div class="row">
                    <div class="col-xs-12">
                        <button class="get-upgarde__button" @click="onButtonClick(cta.link)">
                            {{ cta.copy }}
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "GetUpgrade",
    data() {
        return {
            title: 'Upgrade to the Full Bootcamp',
            text: "Our next cohort starts 3 January 2018",
            cta: {
                copy: "Reserve your spot",
                href: ""
            }
        }
    },
    methods: {
        onButtonClick(link) {
            // navigate to link
            console.log(link);
        }
    }
}
</script>

<style>
.get-upgrade__button {
    list-style-type: none;
}
</style>