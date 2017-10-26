<template>
<section class="hero is-fullheight ">
    <div class="hero-head">
        <header class="nav">
            <div class="container">
                <div class="nav-left">
                    <a class="nav-item" href="">
                        <img class="login-logo is-centered" src="http://www.getstuffdone.io/images/logo.png" alt="">
                    </a>
                </div>
                <span class="nav-toggle">
                <span></span>
                <span></span>
                <span></span>
            </span>
            <div class="nav-right nav-menu">
                <a class="nav-item is-active" href="https://github.com/jamesllewellyn/get-stuff-done">
                    <span class="icon">
                        <i class="fa fa-github"></i>
                    </span>
                </a>
                <span class="nav-item">
                      <a class="button is-orange" href="">
                        <span>Create Team</span>
                      </a>
                </span>
            </div>
            </div>
        </header>
    </div>
    <div class="hero-body">
        <div class="container">
            <div class="columns is-centered">
                <div class="column is-4">
                    <h1 class="title">
                        Login
                    </h1>
                    <div class="box">
                        <form role="form" @submit.prevent>
                            <label for="email" class="label">E-Mail Address</label>
                            <p class="control">
                                <input id="email" type="email" class="input" name="email" :v-model="email" required autofocus>
                            </p>
                            <p class="help is-danger" v-text="getErrors('first_name')"></p>
                            <label for="password" class="label">Password</label>
                            <p class="control">
                                <input id="password" type="password" class="input" name="password" :v-model="password" required>
                            </p>
                            <p class="help is-danger" v-text="getErrors('password')"></p>
                            <p class="control">
                                <button class="button is-primary">Submit</button>
                            </p>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<script>
    export default {
        name: 'log-in',
        data() {
            return{
                'email': '',
                'password' : ''
            }
        },
        methods: {
            /** method to get form field errors **/
            getErrors(fieldName) {
//                return store.getters.getFormErrors(fieldName);
            }
        }
    }
</script>