<template>
    <div>

        <div class="mbile">
            <img style="height:125px" src="../assets/download.png">

            <img style="margin-left:10%; height:100px" src="../assets/download.jpg">
        </div>
        <div class="nav">
            <div class="l">
                <img src="../assets/download.png">
            </div>



            <div class="r">
                <img src="../assets/download.jpg">
            </div>
        </div>

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
         <footer class="footer">
                <p>&copy; Powered by Dic</p>
            </footer>
    </div>
</template>


<script>
export default {
    
}
</script>



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
    position:absolute;
   bottom:0;
   width:100%;
   height:auto;   /* Height of the footer */
   background:royalblue;
}
.footer p{
    margin-top:2%;
    margin-bottom: 2%;
    text-align:center;
    font-size:20px;
    color:white
}.mbile{
    display: none;
}
    /*-- Mobile Devices --*/
@media screen and (max-width: 480px) {
.content{
    display:block;
}
.footer{
    display:none;
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
    height:150px;
    width:300px
}


}
/* -----Tablets- */
@media screen and (max-width: 768px) {
.footer{
    display:none;
}
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