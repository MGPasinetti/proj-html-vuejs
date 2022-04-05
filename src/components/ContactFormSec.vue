<template>
  <section class="contact-form-sec">
      <div class="container-sec jumbotron">
            <div class="header-sec">
                <h2>Contact with our team</h2>
                <small>If you are planning on developing a product landing.</small>
            </div>
            <div>
                <!-- COL-LEFT -->
                <div class="mapouter">
                    <div class="gmap_canvas">
                        <iframe width="450" height="300" id="gmap_canvas" src="https://maps.google.com/maps?q=san%20francisco%20california%2094129%20storey%20ave&t=&z=15&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
                        <a href="https://123movies-to.org"></a>
                        <a href="https://www.embedgooglemap.net"></a>
                    </div>
                </div>

                <!-- COL-RIGHT -->
                <div class="contact-col">
                    <img class="logo" src="../assets/img/35.png" alt="SofBox logo">
                    <span>9840 Shore St. Fond Du Lac, WI 54935</span>
                    <small>0 1223 456 789 <br> mail@sofbox.com</small>
                    <div class="social-icons">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter"></i></a>
                        <a href="#"><i class="fa-brands fa-github"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                    <form action="" class="form-group">
                        <h3>Get in Touch</h3>
                        <div class="name-mail">
                            <input type="text" placeholder="Your Name">
                            <input type="email" placeholder="Your Email">
                        </div>
                        <input type="text" placeholder="Your Subject">
                        <textarea name="message" form="usrform" placeholder="Your Message"></textarea>
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
    @include col-layout($direction: column, $align: center);

    div:last-child {
        display: flex;
        width: 100%;
        gap: .5rem;

        // COL-LEFT
        .mapouter {
            position:relative;
            text-align:right;
            height: 350px;
            width: 450px;

            .gmap_canvas {
                overflow:hidden;
                background:none!important;
                height: 350px;
                width: 450px;
            }
        }

        // COL-RIGHT
        .contact-col {
            display: flex;
            flex-direction: column;


            img {
                width: 6rem;
                margin-bottom: 2rem;
            }

            span {
                font-weight: 400;
                font-size: 16px;
                margin-bottom: 1rem;
            }

            
            .social-icons {
                margin-top: -1rem;
                display: flex;
                gap: .3rem;
                margin-bottom: 1.5rem;

                a {
                    width: 25px;
                    height: 25px;
                    @include flex-layout($justify: center, $align: center, $wrap: wrap);
                    border: 1px solid $border_color_whitesmoke2;
                    border-radius: 3px;

                    i {
                        color: $txt_color_blue;
                        font-size: 12px;
                    }
                }
            } 
                

            .form-group {
                @include col-layout($direction: column, $align: flex-start);
                gap: 1.5rem;

                h3 {
                    margin-bottom: -.5rem;
                }

                .name-mail {
                    width: 100%;
                    @include flex-layout($justify: space-between, $align: center, $wrap: nowrap);
                    gap: 1.5rem;

                    input {
                        flex-grow: 1;
                    }
                }

                input {
                    padding: .5rem;
                    font-size: 12px;
                    width: 100%;
                    border: 1px solid $border_color_whitesmoke2;
                    border-radius: 3px;
                }

                textarea {
                    padding: .5rem;
                    font-size: 12px;
                    width: 100%;
                    height: 150px;
                    border: 1px solid $border_color_whitesmoke2;
                    border-radius: 3px;
                }

            }
        }
    }
}
</style>