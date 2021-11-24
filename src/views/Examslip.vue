<template>
    <div>

        <div class="content">



            <div class="body">


                <!-------header--------->
                <div class="header">
                     <img height="125px" src="../assets/download.png">

                     <img class="iii" height="115px" src="../assets/download.jpg">
                </div>

                

                <h4>Examination Slip</h4>

                <!------------>



                <div class="user">


                    <!------------details ---------->
                    <div class="left">
                        <p>Name:</p>
                        <p>Candidate Identification Number:</p>
                        <p>Post Applied For:</p>
                        
                    </div>
                    <!------------->




                    <!-----Profile picture------>
                    <div class="right">
                        <i class="fa fa-user"></i>
                    </div>
                </div>
                <!----------------->



                <!--------Exams------>
                <div class="exams">
                    <p>Written Essay:</p>

                <p>Computer Based Essay:</p>

                <p>Oral Interview:</p>

                <p>Development Plan:</p>
                </div>

                <!---------------->




                <!------------------->
<div class="bottom">
    <div class="L">
        <p>
            Applicants Signature
        </p>
    </div>


    <div class ="R">
        <p>HOD's Signature</p>
    </div>
</div>

<!-------------->



            </div>
        </div>

        <!-----------footer------>

        <div class="footer">
            <p>Powered by DIC &COPY; 2021</p>
        </div>

        <!------------>
    </div>
</template>


<script>
export default {
    
}
</script>

<!-------styling---->
<style scoped>
body{
    overflow-x:;
}
.header{
    height: 150px;
    display:flex;
}
.header .iii{
    margin-left:35%
}
.content{
    background:white;
    margin-left:35%;
    height:auto;
    margin-top:5vh;
    width:35%;
   
    border:2px solid steelblue
}
.content h4{
    text-align: center;
}
.body .header{
    display:flex;
}
.user{
    display:flex;
}
.user .left{
    width:70%;
    margin-left:5%
}
.user .right{
    width:25%;
}
.user .right i{
    margin-top:15%;
    font-size: 75px;
}
.left p{
    
    font-size: 16px;
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
.bottom{
    
    margin-bottom:0%;
    margin-top:30vh;
    margin-left:10%;
    display:flex;
}
.bottom p{
    font-size: 16px;
    text-align: center;
    font-weight: 600;
}
.bottom .L{
    width:10%;
}
.bottom .R{

    margin-left:60%;
    width:10%
}
.exams{
    margin-left:5%;
    margin-top:2%;
    font-weight: 600;
}
.footer{
    margin-top:8vh;
    background:steelblue;
    height: auto;
    font-size: 20px;
    overflow-y: hidden;
    width:100%;
    color:white;
}
.footer p{
    text-align: center;
    padding-top:2% !important;
    padding-bottom:2% !important
}

/*-- Mobile Devices --*/
@media screen and (max-width: 480px) {
    .content{
        width:100% !important;
        margin-left:0% !important;
        margin-top:2vh;
    }
    .bottom p{
        font-size:12px;
    }
    .left p{
        font-size: 12PX;;
    }
    #courses{
        font-size:12px;
        margin-left:5%
    }
    .header .iii{
    margin-left:15% !important;
    
}
    
}
/* -----Tablets- */
@media screen and (max-width: 768px) {
    .content{
        width:80%;
        margin-left:10%
    }
    .header .iii{
        margin-left:50%
    }
    .footer{
    margin-top:13vh;
    }
}
</style>