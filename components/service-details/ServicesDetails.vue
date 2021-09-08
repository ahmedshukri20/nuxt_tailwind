<template>
    <div class="services-details-area ptb-80">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 services-details">
                    <div class="services-details-desc">
                        <h3>Incredible Infrastructure</h3>
                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry’s standard dummy text ever since the 1500s, when an unknown printer.</p>

                        <p>Took a galley of type and scrambled it to make a type specimen book. survived not only five centuries, but also the leap into electronic remaining. Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry’s standard dummy text ever since the 1500s, when an unknown printer when an unknown.</p>
                    </div>
                </div>

                <div class="col-lg-6 services-details-image">
                    <img src="~/assets/img/services-details-image/1.png" class="wow fadeInUp" v-wow alt="image">
                </div>
            </div>

            <div class="separate"></div>

            <div class="row align-items-center">
                <div class="col-lg-6 services-details-image">
                    <img src="~/assets/img/services-details-image/2.png" class="wow fadeInUp" v-wow alt="image">
                </div>

                <div class="col-lg-6 services-details">
                    <div class="services-details-desc">
                        <p>Took a galley of type and scrambled it to make a type specimen book. survived not only five centuries, but also the leap into electronic remaining. Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry’s standard dummy text ever since the 1500s, when an unknown printer when an unknown.</p>

                        <div class="services-details-accordion">
                            <VueFaqAccordion 
                                :items="myItems"
                            />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import VueFaqAccordion from 'vue-faq-accordion';
export default {
	name: 'ServicesDetails',
	components: {
        VueFaqAccordion
    },
    data() {
        return {
            myItems: [
                {
                    title: 'How many time zones are there in all?',
                    value: 'Given a 24-hour day and 360 degrees of longitude around the Earth'
                },
                {
                    title: 'How long is a day and year on Venus?',
                    value: 'Venus takes 224.7 Earth days to complete one orbit around the Sun.'
                },
                {
                    title: 'What animal smells like popcorn?',
                    value: 'Binturongs smell like popcorn.'
                }
            ]
        }
    }
}
</script>