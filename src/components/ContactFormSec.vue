<template>
  <section class="contact-form-sec">
      <div class="container-sec">
            <h1>Contact with our team</h1>
            <small>If you are planning on developing a product landing.</small>
            <div>
                <!-- COL-LEFT -->
                <img src="../assets/img/StaticMapService.GetMapIma.png" alt="map">

                <!-- COL-RIGHT -->
                <div class="contact-col">
                    <img src="../assets/img/35.png" alt="SofBox logo">
                    <span>9840 Shore St. Fond Du Lac, WI 54935</span>
                    <small>0 1223 456 789 <br> mail@sofbox.com</small>
                    <div class="social-icons">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter"></i></a>
                        <a href="#"><i class="fa-brands fa-github"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                    <form action="" class="form-group">
                        <h1>Get in Touch</h1>
                        <div class="name-mail">
                            <input type="text" placeholder="Your Name">
                            <input type="text" placeholder="Your Email">
                        </div>
                        <input type="text" placeholder="Your Subject">
                        <input type="text" placeholder="Your Message">
                        <button>Send Message</button>
                    </form>
                </div>
            </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'ContactFormSec',
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.container-sec {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 500px;

    div {
        display: flex;
        width: 100%;

        .contact-col {
            display: flex;
            flex-direction: column;

            img {
                width: 8rem;
            }

            .social-icons i {
                color: $txt_color_blue;
            }

            .form-group {
                display: flex;
                flex-direction: column;
            }
        }
    }
}
</style>