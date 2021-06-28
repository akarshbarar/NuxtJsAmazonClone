<template> 
    <div class="admindashboard">
        <nuxt-link to="/">
            <img class="admindashboard__logo" src="http://pngimg.com/uploads/amazon/amazon_PNG11.png"/>


        </nuxt-link>
        <div class="admindashboard__container">
            <h1>Add Element</h1>
            <form>
                <h5>Title</h5>
                <input type="text" placeholder="Enter Title"/>
                 <h5>Description</h5>
                <input type="text" placeholder="Enter Description"/>
                 <h5>Price</h5>
                <input type="text" placeholder="Enter Price"/>
                 <h5>Rating</h5>
                <input type="text" placeholder="Enter Rating"/>
                 <h5>Image URL</h5>
                <input type="text" placeholder="Enter Image URL"/>

                <button type="submit" class="admindashboard__submitButton">Add</button>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.admindashboard{
    background-color: black;
    color: white;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.admindashboard__logo{
    margin: 20px auto;
    object-fit: contain;
    width: 100px;
}
.admindashboard__container{
    width: 300px;
    height: fit-content;
    display: flex;
    flex-direction: column;
    border-radius: 5px;
    border: 1px solid lightgray;
    padding: 20px;
}

.admindashboard__container > h1{
    font-weight: 500;
    margin-bottom: 20px;
}
.admindashboard__container > form > h5{
    margin-bottom: 5px;
}
.admindashboard__container >form > input{
    height: 30px;
    margin-bottom: 10px;
    background-color: white;
    width: 90%;
}
.admindashboard__submitButton{
    border-radius: 2px;
    width: 100%;
    height: 30px;
    border-top: 100px ;
    border: 1px solid;
    border-color: darkgray;
}
</style>