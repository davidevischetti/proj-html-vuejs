<template>
<section>
 <div class="sp-container">
    <h5>SEND A MESSAGE</h5>
    <h2>Get in<div class="special-text">Touch</div></h2>
    <p>We wil respond to your messag as soon as possible&period;</p>

    <form>
        <input type="text" placeholder="Name" required>
        <input type="email" placeholder="Email" required>
        <input type="tel" placeholder="Phone" required maxlength="12">
        <input type="text" placeholder="More info" >
        <textarea name="message" id="message" placeholder="Message" required maxlength="400"></textarea>
        <button class="btn btn-hover">SEND</button>
    </form>
 </div>
 <div id="contact-info">
    <h3>Example Inc.</h3>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit Lorem ipsum dolor</p>
    <a href="#">
        <i><font-awesome-icon icon="fa-solid fa-phone"/></i>
        <span>&plus;1 &lpar;305&rpar; 1234&hyphen;5678</span>
    </a>
    <a href="#">
        <i><font-awesome-icon icon="fa-solid fa-envelope"/></i>
        <span>hello&commat;example&period;com</span>
    </a>
    <a href="#">
        <i><font-awesome-icon icon="fa-solid fa-location-dot"/></i>
        <span>Main Avenue&comma; 987</span>
    </a>
    <a href="https://www.google.com/maps/place/987+Main+Ave,+Schenectady,+NY+12303,+Stati+Uniti/@42.7988841,-73.9492612,17z/data=!3m1!4b1!4m5!3m4!1s0x89de71fad8f50ff9:0x4d5e6cc850a21df4!8m2!3d42.7988802!4d-73.9470725" target="_blank"><button class="btn">VIEW MAP</button></a>
 </div>
</section>
</template>

<script>
export default {
    name: "ContactSection",
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    width: 100%;
    display: flex;

    .sp-container {
        width: 60%;

        h5 {
            color: #54b0c1;
            width: 100%;
        }

        h2 {
            font-size: 40px;
            width: 100%;
            margin: 20px 0;

            .special-text {
                color: #058283;
                background-color: #d5e7e8;
                margin-left: 10px;
            }
        }

        p {
        color: #666;
        font-size: 15px;
        width: 70%;
        }

        form {
            padding: 30px 0;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;

            input {
                width: 49%;
                margin: 5px 0;
                height: 40px;
                border: none;
                background-color: #ececec;
                padding: 10px;
                border-radius: 3px;

                &::placeholder {
                    color: #888;
                }
            }

            #message {
                width: 100%;
                margin: 5px 0;
                height: 120px;
                border: none;
                background-color: #ececec;
                padding: 10px;
                border-radius: 3px;

                &::placeholder {
                    color: #888;
                }
            }

            .btn {
                margin-top: 20px;
            }
        }
    }

    #contact-info {
        width: 40%;
        padding: 80px 30px;
        display: flex;
        flex-wrap: wrap;
        align-content: flex-start;

        h3 {
            width: 100%;
            margin-bottom: 20px;
        }

        p {
            font-size: 12px;
            color: #666;
            width: 51%;
            margin-bottom: 20px;
        }

        a {
            color: #058284;
            font-size: 12px;
            display: flex;
            align-items: center;
            width: 100%;
            margin-top: 20px;

            i {
                margin-right: 10px;
                background-color: #d5e7e8;
                width: 30px;
                height: 30px;
                display: flex;
                justify-content: center;
                align-items: center;
                border-radius: 50%;
            }
        }
    }
}
</style>
