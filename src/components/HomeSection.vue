<template>
    <div class="home">
      <div class="fcontainer">
        <H1>INVEST</H1>
        <h1>&#x2022;&nbsp;&nbsp;INSPIRE</h1>
        <h1>&#x2022;&nbsp;&nbsp;IMPACT</h1>
      </div>
      <p class="quote">Our team of experts specializes in wide software development and more.</p>
      <button class="reach">GET CONNECTED</button>
    </div>
    <div class="cardcontainer">
      <el-row >
        <el-col :span="8">
          <el-card class="card" shadow="never"></el-card>
        </el-col>
        <el-col class="midcol" :span="8">
          <el-card class="card" shadow="never"></el-card>
        </el-col>
        <el-col :span="8">
          <el-card class="card" shadow="never"></el-card>
        </el-col>
      </el-row>
    </div>
</template>
    
    <style lang="scss">
    body{
      background-color:  #131A2C;
    }
    h1{
      font-size: 3vw;
    }
    
    .el-col-8{
      height: 30vw;
      display: flex;
      align-items:end;
    }
    
    .cardcontainer{
      margin-left: 5%;
      margin-right: 5%;
      margin-top: 10px;
      margin-bottom: 5%;
      .midcol{
        align-items: start;
      }
    }
    
    .card{
      background-color: #3b4a7b !important;
      border: none !important;
      border-radius: 8% !important;
      height: 80%;
      width: 80%;
      margin-left: 10%;
      filter: drop-shadow(4px 6px 56px #385ae3);
    }
    
    .quote{
      margin-bottom: 2%;
      font-size: 1vw;
    }
    
    .home{
      // height: 50vh;
      min-height: 30vw;
      color: white;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      
    }
    .fcontainer{
      display: flex;
      
      border-bottom: 0;
      h1{
        padding: 5px;
        margin: 5px;
      }
    
    }
    @media only screen and (max-width:600px){
      h1{
          font-size: 25px;
        }
      .quote{
          margin-bottom: 2%;
          font-size: 12px;
        }
        .home{
          margin-top: 100px;
          margin-bottom: 50px;
        }
    
    }
    
    @media only screen and (max-width:400px){
      h1{
          font-size: 20px;
        }
      .quote{
          margin-bottom: 2%;
          font-size: 8px;
        }
        .home{
          margin-top: 100px;
          margin-bottom: 50px;
    
        }
    
    }
    
    
    </style>