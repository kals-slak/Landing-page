<script setup>
const url= "https://www.zdnet.com/a/img/resize/da370d5ee49d8a058b310a1dab8930ee95f71c2b/2022/07/28/91abefc8-43b0-4c04-8c11-4585a9ed270c/a-man-looking-at-his-smartphone-while-sitting-at-a-computer-in-his-home-office.jpg?auto=webp&width=1280";

</script>

<template>
    <div class="services">
        <div class="sheading">
            <el-divider direction="vertical" class="line"/>
            <span>Comprehensive suite of Services</span>
        </div>
        <div class="sitems">
                <el-row :gutter="2" v-for="j in 2" :key="j">
                    <el-col :xs="24" :sm="12" v-for="i in 2" :key="i">
                        <el-card class="servicecard" shadow="never"></el-card>
                         <h4>Application support</h4>
                         <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
                    </el-col>
                </el-row>
        </div>
    </div>
    <div class="ourservices">
        <div class="ourheading">
            <h1>Our Services</h1>
        </div>
        <div class="items">
            <div class="service">
                <div class="serimg">
                    <el-image style="width: 70%; height: 90%;" :src="url" fit="fill" />
                </div>
                <h3>Application Development</h3>
                <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
            </div>
            <div class="service">
                <div class="serimg">
                    <el-image style="width: 70%; height: 90%;" :src="url" fit="fill" />
                </div>
                <h3>Application Development</h3>
                <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
            </div>
            <div class="service">
                <div class="serimg">
                    <el-image style="width: 70%; height: 90%;" :src="url" fit="fill" />
                </div>
                <h3>Application Development</h3>
                <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
            </div>
        </div>

    </div>
</template>

<style lang="scss">

.ourservices{
    background-color: white;
    color: black;
    height: 100vh;
    .ourheading{
        h1{
            margin: 50px;
            margin-bottom: 0;
            font-size: x-large;
        }
        display: flex;
        align-items: center;
        justify-content: center;
    }
    
    .items{
        height: 90%;
        margin-bottom: 40px;
    }
    .service{
        margin-bottom: 30px;
        display: flex;
        flex-direction: column;
        align-items: center;
        
        .serimg{
            display: flex;
            justify-content: center;
            align-items: center;
            height: 70%;
            padding: 10px;
        }
        *{
            margin-bottom: 10px;
        }
        
        p{
            width: 70%;
            padding-top: 0;
            text-align: center;
        }
    }
    .items{
        display: flex;
        margin-bottom: 20px;
    }
}

.services{
    height: 70vh;
    color: white;
    display: flex;
    .servicecard{
        width: 50px;
        height: 50px;
        background-color: #7784ac;
        border: none;
        filter: drop-shadow(4px 6px 56px #385ae3);
    }
    .sitems{
        margin: 5%;
        width: 70%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        .el-col{
            padding: 25px;
            p{
                width: 62%;
                color: #bbbdc2;
                font-size: small;
            }
            h4{
                color: #478eca;
                width: 80%;
            }
            *{
                margin-bottom: 15px;
            }
        }
    }
    .sheading{
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        span{
            font-size: 2vw;
            font-weight: bold;
            width: 80%;
        }
        .line{
            height: 5vw;
            width: 2px;
            background-color: #51a4de;
        }
    }
}

// @media only screen and (max-width:800px){
//     .services{
//         flex-direction: ;
//     }
// }

@media only screen and (max-width:800px)
{
    .ourservices{
        height: auto;
    }
    .items{
        flex-direction: column;
        margin: 0;
    }
    .services{
        height: auto;
        margin-top: 5%;
        flex-direction: column;
        .sitems{
            justify-content: center;
            width: auto;
            *{
                margin-left: 2%;
            }
            .el-col p{
                width: 80% !important;
                margin: none;
            }
            .el-col{
                margin: none;
            }
        }

        .sheading{
            margin-left: 8%;
            margin-top: 5%;
            width: 80%;
            span{
                font-size:xx-large;
                width: 100%;
            }
            .line{
                height: 100px;

            }
        }
    }
}
</style>