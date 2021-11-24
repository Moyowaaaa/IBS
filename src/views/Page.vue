<template>
    <div>

        <!---------mobile navbar---->
        <div class="mbile">
            <img style="height:125px" src="../assets/download.png">

            <img style="margin-left:10%; height:100px" src="../assets/download.jpg">
        </div>
        <!----------------->



        <!------NavBar---->
        <div class="nav">
            <div class="l">
                <img src="../assets/download.png">
            </div>



            <div class="r">
                <img src="../assets/download.jpg">
            </div>
        </div>
        <!------------->


        <!------content----->
        <h2>Strategic Recruitment and ...... of TOP-LEVEL Management openings in the Civil Service</h2>

        <div class="content">
            <div class="L">
                <img src="../assets/downloadd.jpg">
            </div>


            <div class="R">
                <div class="form">
                    <h3>Application</h3>
                    <br>
                    <br>
                    <label>Name</label>
                    <br>
                    <input type="text">
                    <br>
                    <label>Password</label>
                    <br>
                    <input type="password">
                    <br>
                    <p>Forgot Password?</p>
                    <br>
                    <button>Submit</button>
                </div>
            </div>


           
        </div>

        <!----------->

        <!------footer------>
        <div class="footer">
            <p>Powered by DIC &COPY; 2021</p>
        </div>
        <!--------------->
    </div>
</template>


<script>
export default {
    
}
</script>

<!-------styling---->

<style scoped>

.nav{
    display:flex;
    border-bottom: 1px solid whitesmoke;;
}
.nav img{
    height: 150px; 
}
.nav .l{
    width:20%;
}
.nav .r{
    margin-left:55%;
    width:10%
}
h2{
    text-align: center;
}


.content{
    display:flex;
    width:100%;
}
.content .L{
    padding-top:5%;
    width:30%;
    margin-left:20%;
}
.content .R{
    padding-top:5%;
    width:70%;
}
.form{
    width:90%;
}
input[type="text"], [type="password"]{
    width:30%
}

button{
    width:10%;
    background:royalblue;
    color:white;
    border:none;
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

}.mbile{
    display: none;
}
    /*-- Mobile Devices --*/
@media screen and (max-width: 480px) {
.content{
    display:block;
}

.nav{
    display: none;;
}
.form{
    margin-top:5%;
    margin-left:30% !important;
   
}
input[type="text"], [type="password"]{
    width:70% !important;
}
button{
    width:80%;
    margin-bottom: 5%;
}
h2{
    text-align: center;
    font-size: 18px;
}
.mbile{
    display:flex;
}
.mbile img{
    height:115px !important;
    
}


}
/* -----Tablets- */
@media screen and (max-width: 768px) {

.mbile img{
    height:150px;
    width:200px
}
.form{
    margin-left:10%
}
.content .R{
    padding-top:2%;
}
input[type="text"], [type="password"]{
    width:50%
}
button{
    width:30%
}
.nav .r{
    margin-left:40%;
    width:10%
}
.nav .r img{
    width:300px;
    height:125px
}
.content .L{
    padding-top:5%;
    width:30%;
    margin-left:15%;
}
}

</style>