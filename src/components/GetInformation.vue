<template>
    <div class="get-information container">
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
                        <button class="get-information__button" @click="onButtonClick(cta.link)">
                            {{ cta.copy }}
                        </button>
                    </div>
                </div>
                <div class="row">
                    <div class="col-xs-12">
                        <button class="get-information__button" @click="onButtonClick(cta.link)">
                            {{ cta2.copy }}
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "GetInformation",
    data() {
        return {
            title: 'Get more information',
            text: "We're ready to help with any question you may have about our Bootcamps and Mentor Support",
            cta: {
                copy: "Book a call",
                href: ""
            },
            cta2: {
                copy: "Join an info session",
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
.get-information__button {
    list-style-type: none;
}
</style>