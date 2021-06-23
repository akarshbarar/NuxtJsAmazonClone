<template>
    <div class="header">
        <nuxt-link to="/">
            <img src="http://pngimg.com/uploads/amazon/amazon_PNG11.png"
                class="header__logo" alt="/"/>
        </nuxt-link>

        <div class="header__search">
            <input class="header__searchInput" type="text" placeholder="Search an Item"/>
        </div>

        <div class="header__nav">
            <nuxt-link to="/login" class="header__link">
            <div class="header__option">
                <span class="header__optionLineOne">Hello</span>
                <span class="header__optionLineTwo">Sigin</span>
            </div>
            </nuxt-link>

            <nuxt-link to="/" class="header__link">
                <div class="header__option">
                    <span class="header__optionLineOne">Return</span>
                    <span class="header__optionLineTwo">Prime</span>
                </div>
            </nuxt-link>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>

<style scoped>
.header{
   background-color: #131921;
   display: flex;
   align-items: center;
   width: 100%; 
}
.header__search{
    display: flex;
    align-items: center;
    flex: 1;

    height: 20px;
}
.header__searchInput{
    height: 15px;
    padding: 10px;
    width: 100%;
    border: none;
}
.header__logo{
    object-fit: contain;
    margin-top: 10px;
    margin-left: 20px;
    margin-right: 20px;
    cursor: pointer;
    width: 100px;
}
.header__option{
    display: flex;
    flex-direction: column;
    margin-left: 10px;
    margin-right: 10px;
}
.header__link{
    color: white;
    text-decoration: none;
}
.header__nav{
    display: flex;
    justify-content: space-evenly;
}

</style>