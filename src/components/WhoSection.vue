<template>
    <div class="who">
        <div class="contentcontainer">
            <div class="content">
                <h5>WHO ARE WE?</h5>
                <h3>Your partner in navigating the digital world</h3>
                <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
                <el-button type="primary" plain>Learn More</el-button>
            </div>     
        </div>
        <div class="imagecontainer">
            <el-image style="width: 70%; height: 80%;" :src="url" fit="fill" />
        </div>
    </div>
    <div class="who" id="second">
        <div class="imagecontainer">
           <!-- <div class="image">
                <div class="overlay"></div>
           </div> -->
            <el-image style="width: 70%; height: 80%;" :src="url1" fit="fill" />
        </div>
        <div class="contentcontainer" >
            <div class="content">
                <h5>WHY CHOOSE US?</h5>
                <h3>Experience excellence in IT solutions with us</h3>
                <p>Team of experienced IT professionals dedicated to help business of all sizes achieve their digital potential</p>
                <el-button type="primary" plain>Learn More</el-button>
            </div>     
        </div>
    </div>
</template>

<style lang="scss">


    // .overlay {
    //     width: 100%;
    //     height: 100%;
    //     background-color: rgba(60, 67, 130, 0.811);
        
    //   }
    //   .image {
    //     width: 70%;
    //     height: 80%;
    //     margin-bottom: 20px;
    //     background-image: url('https://img.freepik.com/premium-photo/hand-holding-game-controller_9563-296.jpg?w=2000');
    //     background-position: center;
    //     background-size: cover;
    //     background-repeat: no-repeat;
       
    //   }
.contentcontainer{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50%;
    .content{
        width:80% ;
        *{
            margin: 30px;
        }
        p{
            width: 60%;
            font-size: 1.3vw;
        }
        h3{
            font-size: 2.5vw;
            color: #224996;
            
        }
        h5{
            font-size: 1.5vw;
        }

    }
}

.who{
    background-color: white;
    display: flex;
    height: 700px;
}
.imagecontainer{
    width: 50%;
    display: flex;
    justify-content: center;
    align-items: center;


}

@media only screen and (max-width:600px){
     .who{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
     }
     .imagecontainer{
        width: 100%;
        margin: 10%;
        
     }
     .contentcontainer{
        width: 100%;
        .content{
            width:100% ;
            margin: 8%;
            margin-top: 12%;
            margin-bottom: 12%;
        *{
            margin: 10px;
        }
        p{
            width: 80%;
            font-size: 15px;
        }
        h3{
            font-size: 25px;
            color: #224996;
            
        }
        h5{
            font-size: 20px;
        }

        }
     }
     .who{
        height:auto;
     }
     #second{
        display: flex;
        flex-direction: column-reverse;
        justify-content: center;
        align-items: center;
     }
    
    }

</style>

<script setup>
const url= "https://www.zdnet.com/a/img/resize/da370d5ee49d8a058b310a1dab8930ee95f71c2b/2022/07/28/91abefc8-43b0-4c04-8c11-4585a9ed270c/a-man-looking-at-his-smartphone-while-sitting-at-a-computer-in-his-home-office.jpg?auto=webp&width=1280";
const url1= "https://img.freepik.com/premium-photo/hand-holding-game-controller_9563-296.jpg?w=2000";
</script>