<template>
    <div class="footer">
        <div class="sendus">
            <el-divider direction="vertical" class="line"/>
            <span>Send us a Message</span>
        </div>
        <div class="addresscontainer">
            <div class="address">
            <p>
                123 Anywhere St.. Any City Any State, Country (123) 456 7890
            </p>
            <h3>Sidepash@gmail.com</h3>
                <div class="cardss">
                    <el-row :gutter="2" >
                        <el-col :xs="8" :sm="8" v-for="i in 3" :key="i">
                            <el-card class="servicecard" shadow="never"></el-card>
                        </el-col>
                    </el-row>
                </div>
            </div>

        </div>
        
    </div>
</template>
<style lang="scss"> 
.footer{
    display: flex;
    .addresscontainer{
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        p{
            font-size: x-large;
            margin-bottom: 30px;
        }
        h3{
            color: #6fafe1;
        }
    }
    .address{
        *{
            margin-bottom: 20px;
        }
        .cardss{
            width: 20%;
        }
        display: flex;
        flex-direction: column;
        justify-content: center;
        p{
            width: 50%;
        }
    }
    .servicecard{
        width: 25px;
        height: 25px;
        background-color: #7784ac;
        border: none;
    }
    height: 70vh;
    background-image: url("https://home.heinonline.org/blog/wp-content/uploads/2021/05/ToTW-1.png");
    background-size: cover;
    color: white;
    .sendus{
        height: 60%;
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        span{
            font-size: 3vw;
            font-weight: bold;
            width: 50%;
        }
        .line{
            height: 5vw;
            width: 2px;
            background-color: #51a4de;
        }
    }
}

@media only screen and (max-width:400px){
    .addresscontainer{
            width: 80%;
            p{
                width: 100%;
            }
        }
        .sendus{
            width: 100%;
            span{
                font-size:40px;
                width: 100%;
            }
            .line{
                height: 100px;

            }
        }
        .cardss{
            .el-row{
            width: 100px;
        }
        }
        

}

@media only screen and (max-width:800px){
    .footer{
        margin: 0;
        padding: 0;
        flex-direction: column;
        // justify-content: center;
        align-items: center;
        width: 100%;
        
        .addresscontainer{
            width: 80%;
            p{
                width: 80%;
            }
        }
        .sendus{
            width: 100%;
            span{
                font-size:40px;
                width: 80%;
            }
            .line{
                height: 100px;

            }
        }
    }
}

</style>