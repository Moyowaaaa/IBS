<template>
    <div class="admin"> 


<div class="mob">
  <div class="ML">
                        <img src="../assets/download.png">
                    </div>

                    <div class="MR">
                       <img  height="50px" src="../assets/download.jpg">
                      <span class="mbutton" style="font-size:40px;cursor:pointer" @click="openNav">
  &#9776;</span>
                      </div>

                      

</div>

 <div id ="mobile" class="mobilenav">
      <a href="javascript:void(0)" class="closebtn" @click="closeNav">&times;</a>
      <div class="ml"  @click="closeNav">
  
         <a>Login Time</a>
        <a >View Applicant</a>
        <a >Enter Score 1</a>
        <a >Enter Score 2</a>
        <a>Enter Score 3</a>
        <a>Enter Score 4</a>
        <a>Send Mail</a>
        <a>Send Sms</a>
        <a>Settings</a>
      </div>
  </div>








        <div class="main">

            <div class="left">

                <div class="side">


                    <div >
                        <img src="../assets/download.png">
                    </div>

                    <div class="links">
                        <p>LOGIN TIME</p>
                    </div>

                    <div class="links">
                        <router-link to="/"><p>View Applicant</p></router-link>
                    </div>

                    <div class="links">
                        <p>Enter Score 1</p>
                    </div>

                    <div class="links">
                        <p>Enter Score 2</p>
                    </div>

                    <div class="links">
                        <p>Enter Score 3</p>
                    </div>

                    <div class="links">
                        <p>Enter Score 4</p>
                    </div>


                    <div class="links">
                        <p>Send Mail</p>
                    </div>


                    <div class="links">
                        <p>Send Sms</p>
                    </div>

                    <div class="links">
                       
                    </div>

                    <div class="links">
                        <p>Settings</p>
                    </div>
                </div>
            </div>



            <div class="right">


                <div class="header">
                    <div class="L">
                        <h1>TITLE</h1>
                    </div>

                    <div class="R">
                        <img src="../assets/download.jpg">
                    </div>

                    
                </div>


                <div class="content">
                    <h2>Welcome Admin</h2>
                </div>


<div class="ttt" style="overflow-x: auto;">
<table>
  <tr>
     <th>Id</th>
    <th>Name</th>
    <th>Position Applied for</th>

    <th>Written Essay Score</th>
    <th>Score 2</th>
    <th>Score 3</th>

    <th>Score 4</th>
    <th>Average</th>
    <th>Total</th>
  </tr>
  </table>
  </div>

<!--------------
                                <table id="courses">
  <tr>
    <th>Id</th>
    <th>Name</th>
    <th>Position Applied for</th>

    <th>Written Essay Score</th>
    <th>Score 2</th>
    <th>Score 3</th>

    <th>Score 4</th>
    <th>Average</th>
    <th>Position Applied for</th>

    
    
  </tr>
 
</table>
------->

            </div>



        </div>
        <div class="footer">
            <p>Powered by DIC &COPY; 2021</p>
        </div>
    </div>
</template>


<script>
export default {
  methods:{
  openNav() {
    document.getElementById("mobile").style.width = "100%";
},
closeNav() {
    document.getElementById("mobile").style.width = "0";
}
}
}
</script>

<style scoped>
.nav{
    background:whitesmoke;
    display:flex;
    width:100.5%;
    height:auto;
    margin:-8px;
    overflow-x: hidden;
}
.nav h3{
    font-weight: 600;
    margin: 30px;
    font-size: 20px;

}
.nav .links{
    margin-left:600px;
    font-weight: 600;
    margin: 30px;
    font-size: 20px;
}


.main{
    margin-top:1%;
    width:100%;
    display:flex;
    height: auto;
}
.left{
    width:15%;
    height:auto;
    
}
.left  img, .right img{
  width:150px
}
.right{
    width:85%;
  
}
.header{
    display:flex;
    
}
.header .L{
    width:75%;
    margin-top:5%
}
.header .R{
    width:10%
}
 .L h1{
    text-align: center;
}
.left .side{
    display:block;
}
.side .links{
    height:100px;
    width:100%;
    border:1px solid teal
}
.links p{
    text-align:center;
    margin-top:50px;
}
h2{
    font-size: 30px;
    font-weight: 600;
    margin-left:10%
    }
    .footer{
    margin-top:1vh;
    background:steelblue;
    height: auto;
    font-size: 20px;
    overflow-y: hidden;
    width:100%;
    color:white;
}
.footer p{
    text-align: center;
    padding-top:1%;
    padding-bottom:1%

    }.mob , .mobilee{
  display: none;
}

hr{
  width:3.25em
}

.mobilenav {

    height: 100%;
    width: 0;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;
     background:#333b50;
    overflow-x: hidden;
    transition: 0.5s;
    padding-top: 60px;
}

.mobilenav a {
    padding: 2% 8px 8px 32px;
    text-decoration: none;
    font-size: 25px;
    font-weight: 550;
    color: black;
    display: block;
    transition: 0.3s;
}

.mobilenav a:hover {
    color: #f1f1f1;
}

.mobilenav .closebtn {
    position: absolute;
    top: 0;
    right: 25px;
    font-size: 36px;
    margin-left: 50px;
}
.mbutton{
  display:none;
  position:sticky;
  margin-top:5%;
}
.span{
  color:steelblue
}
table {
  border-collapse: collapse;
  width: 90%;
  margin-left:5%;
  margin-top:5%
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}
.content h2{
  font-size: 20px;
  margin-left: 5%;
}

    /*-- Mobile Devices --*/
@media screen and (max-width: 480px) {
.left{
    display:none;
}
  .header, .L, .R{
  
    display:none; 
  }
  .mob{
      display:flex;
  }
.mob .MR{
  Margin-left:40% !important;
  display:flex;
}
.mob .ML img{
  
  height:50px
}
.mobilenav .mobileimg{
  margin-left: 5%
}
.mobilee{
  display: block;
  text-align: center;
}
.mbutton{
  display:block
}
#mobile .ml a{
  padding-top:5%
}

 #mobile .ml{
    width:80%;
    margin-left:2%;
    text-align: center;
  }
  table {
  border-collapse: collapse;
  width: 100%;
  
  margin-top:5%
}
.footer{
    margin-top:70vh !important;
    background:steelblue;
    height: auto;
    font-size: 20px;
    overflow-y: hidden;
    width:100%;
    color:white;
}
}

/* -----Tablets- */
@media screen and (max-width: 768px) {
    .mobilee{
  display: block;
  text-align: center;
}
.mob .MR{
  Margin-left:40%;
  display:flex;
}
.mbutton{
  display:block
}
.mob{
  display:flex;
}
.mob .MR{
  Margin-left:75% 
}
.mob .ML img{
  
  height:50px
}
  .left{
       display:none;
   }
     .header, .L, .R{
   
     display:none; 
   }
    .flex .cont{
    width:70%;
    margin-top:5%
  }
  #mobile .ml{
    width:50%;
    margin-left:25%;
    text-align: center;
  }
  table {
  border-collapse: collapse;
  width: 100%;
  margin-left:5%;
  margin-top:5%
}
.ttt{
    margin-left:5%;
    width:100%
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}
.footer{
    margin-top:75vh;
    background:steelblue;
    height: auto;
    font-size: 20px;
    overflow-y: hidden;
    width:100%;
    color:white;
}
}



</style>