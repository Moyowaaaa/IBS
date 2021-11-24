<template>
  <div>

    <!------mobile Header--->
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
<!------------------>


<!----mobile sidebar--->
  <div id ="mobile" class="mobilenav">
      <a href="javascript:void(0)" class="closebtn" @click="closeNav">&times;</a>
      <div class="ml"  @click="closeNav">
     
         <a>Login Time</a>
        <a >View Profile</a>
        <a >Institutional Materials</a>
        <a href="/ExamSlip">Print Exam Slip</a>
        <a>Complaints and feedback</a>
        <a>FAQs</a>
      </div>
  </div>
  <!------------>







<!----------main contents ---->
    <div class="main">

      <!------left contents----->
      <div class="left">
         <div class="side">


           <!--sidebar------>


                    <div >
                        <img src="../assets/download.png">
                    </div>

                    <div class="links">
                        <p>LOGIN TIME</p>
                    </div>

                    <div class="links">
                        <p>View Profile</p>
                    </div>

                    <div class="links">
                        <p>Institutional Materials</p>
                    </div>

                    <div class="links">
                        <router-link to="/ExamSlip"><p>Print Exam Slip</p></router-link>
                    </div>

                    <div class="links">
                        <p>Complaints and feedback</p>
                    </div>

                    <div class="links">
                        <p>FAQs</p>
                    </div>


                    
                </div>
                <!----------->
      </div>



      <div class="right">
        <!--------right contents--------->
        <div class="header">
                    <div class="L">
                        <h1>TITLE</h1>
                        <hr>
                    </div>

                    <div class="R">
                        <img src="../assets/download.jpg">
                    </div>

                    
                </div>

              

                <div class="content">
                  <br>
                 
                  <p>
                    Dear <span style=font-weight:600>Name of Applicant</span>
                  </p>

                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rerum laboriosam esse neque officia eveniet accusantium, corporis est praesentium, eos obcaecati vero cupiditate quo. Alias ullam reiciendis nulla aspernatur ut quibusdam?</p>
                                  </div>


                                  <div class="flex">


                                    <div class="cont">
                                      <p>Stage 1</p>

                                      <p>Written Essay</p>
                                    </div>

                                      <div class="cont">
                                        <p>Stage 2</p>

                                        <p>Computer Based Test</p>
                                    </div>

                                      <div class="cont">
                                        <p>Stage 3</p>
                                        <p>Oral Interview</p>
                                    </div>

                                      <div class="cont">
                                      <p>Stage 4</p>
                                      <p>Development Plan</p>
                                    </div>


                                  </div>
      </div>
    </div>


    <!-------footer------->
       <div class="footer">
            <p>Powered by DIC &COPY; 2021</p>
        </div>

        <!----------------->
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

<!-------styling---->

<style scoped>
.main{
    width:100%;
    display:flex;
    height: auto;
}
.left{
    width:15%;
    height:auto;
    
}
.right{
    width:85%;
  
}
#courses th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;

  color: black;
  margin-left:25%
}


#courses {
   
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
  margin-left:5%;
}
th{
  border-right: 1px solid black;

}
.content p{
  font-size: 20px;
  margin-left:2%;
}
.flex{
  display: flex;
  flex-wrap: wrap;
}
.flex .cont{
  height:auto;
  width:20%;
  border: 2px solid blue;
  margin-left:15%;
  margin-top:4%
}
.cont p{
  font-size: 25px;
  text-align: center;
  margin-top:1vh;
  padding-top: 2vh;
}
.left  img, .right img{
  width:150px
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
}.header{
    display:flex;
}
.header .L{
    width:75%
}
.header .R{
    width:10%
}
 .L h1{
    text-align: center;
    padding-top:10%;
}
.mob , .mobilee{
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
  margin-top:-1%;
}
.span{
  color:steelblue
}
.footer{
    margin-top:17vh;
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
}



    /*-- Mobile Devices --*/
@media screen and (max-width: 480px) {
   .left{
      display:none;
  }
 
  .content{
    width:100%

  }
  .content p{
    font-size:16px;
    text-align: justify;
    font-weight: 600;
    margin-left:10%;
  }
 .flex {
    display: block;
    flex-wrap: none;;
  }
  .flex .cont{
    width:80% !important;
    margin-left:20% !important;
   
    margin-top:5%
  }
  .header, .L, .R{
  
    display:none; 
  }
  .header .L{

  }
  .R{
    margin-left:-80%
  }
  .cont p{
  font-size: 18px;
  text-align: center;
  margin-top:1vh;
  padding-top: 2vh;

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

}
.mbutton{
  display:block;
  margin-top:1%
}
#mobile .ml a{
  padding-top:5%;
  width:100%;
}
}


/* -----Tablets- */
@media screen and (max-width: 768px) {

  .content{
    width:85%;
    margin-left:7.5%;
  }

.mobilee{
  display: block;
  text-align: center;
}
.mbutton{
  display:block
}
.mob{
  display:flex;
}
.mob .MR{
  Margin-left:70%;
  display:flex;
}
.mob .ML img{
  
  height:50px
}
  .left{
       display:none;
   }
     .header, .L, .R{
   
     display:none; 

   }  .flex .cont{
    width:80% !important;
    margin-left:20% !important;
 
    margin-top:5%
  }
  #mobile .ml{
    width:50%;
    margin-left:25%;
    text-align: center;
  }
}









</style>