<template>
    <div class="login-container">
        <div class="login-box">


            <div class="avatar">
                <img src="../assets/logo.png" alt="">
            </div>


            <div class="form" >


                <el-form :model="form" :rules="rules">

                    <el-form-item prop="userName">
                        <el-input v-model="form.userName" label="" prefix-icon="" ></el-input>
                    </el-form-item>


                    <el-form-item prop="password">
                        <el-input v-model="form.password" label="" prefix-icon="" type="password"></el-input>
                    </el-form-item>
                    <el-form-item class="btn-box">

                        <el-button type="primary">登录</el-button>
                        <el-button type="info">重置</el-button>
                    </el-form-item>

                </el-form>

            </div>


        </div>
    </div>
</template>

<script>

    export default {
        name: "Login",
        data(){

            return {

                form: {

                    userName: "",
                    password: ""







                }


            }



        }


    }
</script>

<style scoped lang="scss">
    .login-container {

        background-color: #2b4b6b;

        height: 100%;

    }

    .login-box {


        width: 450px;
        height: 300px;
        background-color: #fff;
        border-radius: 3px;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);


        .avatar {

            height: 100px;
            width: 100px;
            margin: 0 auto;
            transform: translate(0, -50%);
            border-radius: 50%;
            padding: 10px;
            background-color: #fff;

            img {
                width: 100%;
                height: 100%;
                display: block;
                border-radius: 50%;
                background-color: #bbb;

            }


        }
    }

    .form {


        padding: 0 20px;
        .btn-box{


            display: flex;
            justify-content: center;

        }



    }
</style>