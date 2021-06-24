<template>
    <div class="headerTwo__options">
        <div class="headerTwo__optionDeliver">
            
            <div class="headerTwo__optionDeliverySpan">
                <span>Delivery</span>
                <span>India</span>
            </div>
        </div>

        <div class="headerTwo__optionLink">
            <nuxt-link to="/" class="headerTwo__link">
                <span>Todays Deal</span>
            </nuxt-link>
             <nuxt-link to="/" class="headerTwo__link">
                <span>Customer Service</span>
            </nuxt-link>
             <nuxt-link to="/" class="headerTwo__link">
                <span>Gift Cards</span>
            </nuxt-link>
             <nuxt-link to="/" class="headerTwo__link">
                <span>Registry</span>
            </nuxt-link>
             <nuxt-link to="/" class="headerTwo__link">
                <span>Sell</span>
            </nuxt-link>
        </div>

        <div class="link">
            <span> Amazon's response to Covid-19</span>
        </div>
    </div>
</template>
<script>
    export default {}
</script>

<style scoped>
.link{
    color: white;
}
    .headerTwo__link{
        color:white;
        text-decoration: none;
    }
    .headerTwo{
        color:white;
    }
    .headerTwo__options{
        display: flex;
        justify-content: space-between;
        padding: 10px;
        background-color: #232f3e;
    }
    .headerTwo__optionDeliverySpan{
        display: flex;
        flex-direction: column;
        margin-left: 10px;
        margin-right: 10px;
    }

    .headerTwo__optionDeliver{
        display: flex;
        color:white;
    }
    .headerTwo__optionLinks{
        display: flex;
        justify-content: space-between;
        width: 25%;
    }
</style>
