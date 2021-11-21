<template>
    <div>

        <div class="content">
            <div class="body">
                <div class="header">
                     <img src="../assets/download.png">
                </div>


                <h4>Semester</h4>


                <div class="user">
                    <div class="left">
                        <p>Name:</p>
                        <p>Matric No:</p>
                        <p>Faculty:</p>
                        <p>Department:</p>
                    </div>



                    <div class="right">
                        <i class="fa fa-user"></i>
                    </div>
                </div>



                <table id="courses">
  <tr>
    <th>Course Code</th>
    <th>Course Title</th>
    <th>Course Unit</th>
  </tr>
 
</table>



<div class="bottom">
    <div class="L">
        <p>
            Students Signature
        </p>
    </div>


    <div class ="R">
        <p>HOD's Signature</p>
    </div>
</div>



            </div>
        </div>
    </div>
</template>


<script>
export default {
    
}
</script>


<style scoped>
.header{
    height: 150px;
}
.content{
    background:white;
    margin-left:35%;
    height:auto;
    margin-top:5vh;
    width:35%;
    border:2px solid red
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
    font-weight: 600;
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
    
}
/* -----Tablets- */
@media screen and (max-width: 768px) {
    .content{
        width:80%;
        margin-left:10%
    }
}
</style>