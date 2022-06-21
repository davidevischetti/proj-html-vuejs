<template>
<section class="container">
    <div id="footer-info">

        <!-- LOGO -->
        <img src="../assets/svg/svg-7.svg" alt="logo">

        <p>A Functional HTML Template for Corporate &amp; Business.</p>

        <!-- INFO CONTATTI -->

        <!-- NUMERO -->
        <a href="#">
            <font-awesome-icon icon="fa-solid fa-phone"/>
            <span>&plus;1 &lpar;305&rpar; 1234&hyphen;5678</span>
        </a>

        <!-- EMAIL -->
        <a href="#">
            <font-awesome-icon icon="fa-solid fa-envelope"/>
            <span>hello&commat;example&period;com</span>
        </a>

        <!-- POSIZIONE -->
        <a href="#">
            <font-awesome-icon icon="fa-solid fa-location-dot"/>
            <span>Main Avenue&comma; 987</span>
        </a>

        <button class="btn">GET IN TOUCH</button>

    </div>
     <!-- LISTE LINK FOOTER -->

     <!-- LINK ABOUT -->
     <ul>
        <li><h4>About</h4></li>
        <li v-for="(aboutLink, i) in aboutFooterLinks" :key="i">
            <i><font-awesome-icon icon="fa-solid fa-angle-right"/></i>
            <a href="#">{{aboutLink}}</a>
        </li>
     </ul>

    <!-- LINK SERVICES -->
     <ul>
        <li><h4>Services</h4></li>
        <li v-for="(serviceLink, j) in servicesFooterLinks" :key="j">
            <i><font-awesome-icon icon="fa-solid fa-angle-right"/></i>
            <a href="#">{{serviceLink}}</a>
        </li>
     </ul>

    <!-- LINK SUPPORT -->
     <ul>
        <li><h4>Support</h4></li>
        <li v-for="(supportLink, k) in supportFooterLinks" :key="k">
            <i><font-awesome-icon icon="fa-solid fa-angle-right"/></i>
            <a href="#">{{supportLink}}</a>
        </li>
     </ul>

</section>
</template>

<script>
export default {
    name: "FooterSection",
    data() {
        return {
            // LISTE LINK DEL FOOTER
            aboutFooterLinks: ["The Company", "Institutional", "Social & Events", "Innovation", "Environment", "Technology"],
            servicesFooterLinks: ["Audit & assurance", "Financial Advisory", "Analytics M&A", "Middle Marketing", "Legal Consulting", "Regulatory Risk"],
            supportFooterLinks: ["Responsability", "Terms of Use", "About Cookies", "Privacy Policy", "Accessibility", "Information"]
        };
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    width: 100%;
    background-color: #111117;
    padding-bottom: 80px;
    flex-wrap: wrap;

    // STILE INFORMAZIONI CONTATTI
    #footer-info {
        margin-top: 80px;
        display: flex;
        flex-direction: column;
        align-content: flex-start;
        flex-basis: 24%;
        min-height: 250px;

        img {
            width: 100px;
        }

        p {
            font-size: 12px;
            color: #888;
            margin: 20px 0;
        }

        a {
            color: #888;
            font-size: 12px;
            margin-bottom: 10px;
        }

        .btn {
            color: #fff;
            margin-top: 20px;
            width: fit-content;
            margin-bottom: 80px;
        }

    }

    // STILE LISTE LINKS
    ul {
        flex-basis: 24%;
        background-color: #19191f;
        padding: 30px;
        border-radius: 5px;
        min-height: 250px;

        h4 {
        color: #fff;
        margin-bottom: 20px;
        }

        i {
            color: #888;
            font-size: 12px;
            margin-right: 10px;
        }

        a {
            color: #888;
            font-size: 12px;
            margin-bottom: 10px;
        }

    }
}
</style>
