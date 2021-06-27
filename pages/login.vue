<template>
    <div class="login">
        <nuxt-link to="/">
            <img class="login__logo" src="http://pngimg.com/uploads/amazon/amazon_PNG11.png"/>


        </nuxt-link>
        <div class="login__controller">
            <h1>Sign In</h1>
            <form>
                <h5>Email</h5>
                <input type="email" placeholder="E-mail"/>
                <h5>Password</h5>
                <input type="password" placeholder="Password"/>

                <button type="submit" class="login__signInButton">
                    Sigin
                </button>
            </form>
            <p>By Signing in Yoou agree to Amzaon Clone Condition</p>
            <nuxt-link to="/register">
            <button class="login__registerButton">Create your New Account</button>
            </nuxt-link>
        </div>
    </div>
</template>
<script>
export default {}
</script>
<style scoped>
.login{
    background-color: black;
    color: white;
    height:100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.login__logo{
    margin: 20px auto;
    object-fit: contain;
    width: 100px;

}

.login__controller{
    width: 300px;
    height: fit-content;
    display: flex;
    flex-direction: column;
    border-radius: 5px;
    border: 1px solid lightgray;
    padding: 20px;
}
.login__controller > h1{
    font-weight: 500;
    margin-bottom: 20px;
}

.login__controller > form > h5{
    margin-bottom: 5px;
}

.login__controller > form > input{
    height: 30px;
    margin-bottom: 10px;
    background-color: white;
    width: 90%;
}
.login__controller > p{
    margin-top: 15px;
    font-size: 12px;
}
.login__signInButton{
    background: #f0c14b;
    border-radius: 2px;
    width: 100%;
    height: 30px;
    border: 1px solid;
    margin-top: 10px;
    border-color:#a88734 #9c7e31 #846a29 ;
}
.login__registerButton{
    border-radius: 2px;
    width: 100%;
    height: 30px;
    border-top: 100px;
    border: 1px solid;
    border-color: darkgray;
}
</style>
