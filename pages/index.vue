<template>

    <main>
        <!--? slider Area Start-->
        <div class="slider-bg" v-if="loaded">
            <client-only>
                <carousel :per-page="1" :autoplay="true" :loop="true"
                          :paginationEnabled="true"
                          :navigation-enabled="false"
                          :paginationActiveColor="'#37bbe1'"
                          :autoplayTimeout="4000">
                    <slide>
                        <img src="~/assets/img/home/banner.jpg">
                        <div class="slider-info">
                            <div class="col">
                                <h1>2º Congreso Internacional de Ginecólogos Oncólogos</h1>
                                <h1>Congreso Virtual</h1>
                                <img src="~/assets/img/home/banner1.png" alt="" width="300px">
                                <h2 class="mb-4">13 y 14 de noviembre</h2>
                                <button v-b-modal.modal-login
                                           class="btn">INICIAR SESIÓN
                                </button>
                                <div>
                                    <nuxt-link to="/registro"><p class="movil-center float-right text-white mt-3">Si no estás registrado,<span class="text-lowercase"> hazlo <u class="text-white"><strong>aquí</strong></u></span> </p></nuxt-link>
                                </div>
                            </div>
                        </div>
                    </slide>
                    <!--slide>
                        <img src="~/assets/img/home/banner1.jpg">
                        <div class="slider-info">
                            <div class="col">
                                <h1>JORNADAS ACADÉMICAS VIRTUALES</h1>
                                <img src="~/assets/img/logo/logo_combinado_white.png" alt="">
                                <h2 class="mb-4">del 23 al 25 octubre 2020</h2>
                                <nuxt-link to="/registro"
                                           class="btn">¡Regístrate!
                                </nuxt-link>
                            </div>
                        </div>
                    </slide-->
                </carousel>
            </client-only>
        </div>
        <!-- slider Area End-->
        <!--? About Law Start-->
        <!--section class="about-low-area section-padding2">
            <div class="container">
                <div class="row">
                    <div class="col-lg-6 col-md-12">
                        <div class="about-caption mb-50">
                            <div class="section-tittle mb-35">
                                <h2>Desde 23 de julio</h2>
                            </div>
                            <p>Tenga en cuenta que para 2020 tenemos nuevos requisitos en torno al Congreso virtual. Se
                                requiere una dirección de correo electrónico única para cada individuo para acceder a la
                                plataforma virtual. Sin una dirección de correo electrónico única, el miembro del grupo
                                no podrá obtener acceso al Congreso virtual.</p>

                            <p>Esta dirección de correo electrónico también se utilizará para enviar cualquier
                                correspondencia relevante y acceder a la constancia después del congreso. Proporcionar
                                esta información por adelantado también nos permitirá procesar todos los registros
                                individuales o de grupo de manera eficiente y entregar detalles de inicio de sesión a
                                los registrados de manera oportuna.</p>
                        </div>
                        <div class="row">
                            <div class="col-lg-6 col-md-6 col-sm-6 col-xs-10">
                                <div class="single-caption mb-20">
                                    <div class="caption-icon">
                                        <fa icon="calendar" class="fa-3x" style="color: #26264b"/>
                                    </div>
                                    <div class="caption">
                                        <h5>Fecha</h5>
                                        <p>9 y 10 de octubre</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <a href="http://registro.mastologia.org.mx/" target="_blank" class="btn mt-50">¡Regístrate!</a>
                    </div>
                    <div class="col-lg-6 col-md-12 mt-5">
                        <img src="~/~/assets/images/logo-small.png" class="mt-100 d-block m-auto">
                    </div>
                </div>
            </div>
        </section-->
        <!-- About Law End-->
        <!--? Brand Area Start -->
        <section class="team-area gradient-bg pt-100 pb-100 section-bg">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 info">
                        <!-- Section Tittle -->
                        <div class="section-tittle section-tittle2 mb-50">
                            <div class="section-tittle mb-35">
                                <h2 class="text-center">Estimados, colegas y amigos:</h2>
                            </div>
                            <p class="text-center">
                                A medida que la especialidad de Ginecología Oncológica se posiciona en
el ámbito médico nacional; es el momento perfecto para ver el futuro; ya
nos estamos consolidado como uno de los colegios líder en el campo del
cáncer en la mujer, específicamente las neoplasias de los genitales de la
mujer, de manera única; se han agregado especialistas de diferentes áreas
de especialidad afines como la cirugía oncológica, radioterapia, oncología
médica, principalmente y profesionales de la salud interesados en los
tumores ginecológicos, estamos consolidándonos a nivel nacional para
integrarnos al resto del mundo; al construir una reputación sólida que
seguramente enorgullece a nuestros colegiados.
                            </p>
                            <p class="text-center">
                                En más de medio siglo de existencia de la Ginecología Oncológica,
muchas cosas han cambiado y de forma acelerada cada día que pasa y
necesitamos adaptarnos a esos cambios; la informática digital, con sus
ventajas y desventajas, se ha convertido en la forma primordial de
compartir información; aumentaremos nuestra presencia en redes
sociales para promover la comunicación académica con diferentes
agrupaciones nacionales e internacionales del ámbito, público y privado.
Tenemos la obligación de promover la comunicación nacional e
internacional, así como la difusión del conocimiento; realizar este
congreso puede ser una manera de cerrar esta brecha, mientras
cumplimos con nuestro deber de difundir el conocimiento e involucrar a
la mayoría de los colegiados, residentes y colegas de diferentes países.
Ya somos un colegio reconocido y respetado, donde deben ser parte de él;
en el futuro continuaremos siendo el colegio líder en la salud de las
mujeres con cáncer ginecológico
                            </p>
                            <p class="text-center">
Acad. Dr. Víctor Manuel Vargas Hernández</p>
                        </div>
                    </div>
                    <div class="col-md-6 register">
                        <div class="counter-section">
                            <h1>YA EMPEZAMOS LA CUENTA REGRESIVA</h1>
                            <div class="cd-timer" id="countdown">
                                <client-only>
                                    <countdown :time="countDown">
                                        <template slot-scope="props">
                                            <div class="cd-item">
                                                <span>{{ props.days }}</span>
                                                <p>Días</p>
                                            </div>
                                            <div class="cd-item">
                                                <span>{{ props.hours }}</span>
                                                <p>Hrs</p>
                                            </div>
                                            <div class="cd-item">
                                                <span>{{ props.minutes }}</span>
                                                <p>Min</p>
                                            </div>
                                            <div class="cd-item">
                                                <span>{{ props.seconds }}</span>
                                                <p>Seg</p>
                                            </div>
                                        </template>
                                    </countdown>
                                </client-only>
                            </div>
                        </div>

                        <nuxt-link to="/registro" class="btn mt-50">¡Regístrate!</nuxt-link>
                    </div>

                </div>
            </div>
        </section>
        <!-- Brand Area End -->
        <!--? Blog Area Start -->
        <section class="home-blog-area mt-4 mb-4 pt-4 pb-4">
            <div class="container">
                <h2 class="text-center mb-4 font-weight-bold" style="color:#151762">CENTRO DE ATENCIÓN CMOG 2020</h2>
                <div class="row">
                    <div class="col-md-4 col-lg-4">
                        <a href="https://www.srcongress.mx/cmog/registro_virtual.php" >
                            <div class="congress-content">
                                <img src="~/assets/images/registro_primera_vez.jpg" alt="">
                                <div class="details">
                                    <p class="title">
                                        REGISTRO PRIMERA VEZ
                                    </p>
                                    <p class="subtitle">Acceso sin costo</p>
                                </div>
                            </div>
                        </a>
                    </div>
                    <div class="col-md-4 col-lg-4 ">
                        <a href="#" @click="$bvModal.show('dudas')">
                            <div class="congress-content">
                                <img src="~/assets/images/atencion_duidas.jpg" alt="">
                                <div class="details">
                                    <p class="title">
                                    ATENCIÓN DE DUDAS
                                    </p>
                                    <p class="subtitle"></p>
                                </div>
                            </div>
                        </a>
                    </div>
                    <div class="col-md-4 col-lg-4">
                        <a href="#" @click="$bvModal.show('acceso')">
                            <div class="congress-content">
                                <img src="~/assets/images/problemas_acceso.jpg" alt="">
                                <div class="details">
                                    <p class="title">
                                        PROBLEMAS DE ACCESO
                                    </p>
                                    <p class="subtitle"></p>
                                </div>
                            </div>
                        </a>
                    </div>
                    <div class="col-md-4 col-lg-4 ">
                        <a href="#" @click="openPaymentChat">
                            <div class="congress-content">
                                <img src="~/assets/images/aclaracion_pagos.jpg" alt="">
                                <div class="details">
                                    <p class="title">
                                        ACLARACIÓN DE PAGOS
                                    </p>
                                    <p class="subtitle"></p>
                                </div>
                            </div>
                        </a>
                    </div>
                    <div class="col-md-4 col-lg-4">
                        <a href="/docs/Programa-CMOG03-11.pdf" download="">
                            <div class="congress-content">
                                <img src="~/assets/images/pograma.jpg" alt="">
                                <div class="details">
                                    <p class="title">
                                        DESCARGA EL PROGRAMA
                                    </p>
                                    <p class="subtitle"></p>
                                </div>
                            </div>
                        </a>
                    </div>
                    <!--div class="col-md-6 col-lg-4">
                        <div class="congress-content">
                            <img src="~/assets/images/PRIMER_CONTACTO.jpg" alt="">
                            <div class="details">
                                <p class="title">
                                    <a href="#" @click="$bvModal.show('oncologia')">ONCOLOGÍA PRIMER CONTACTO</a>
                                </p>
                                <p class="subtitle">A partir del 22 de Septiembre</p>
                            </div>
                        </div>
                    </div-->
                    <!--div class="col-md-6 col-lg-4">
                        <div class="congress-content">
                            <img src="~/assets/img/content/eposter_2.jpg" alt="">
                            <div class="details">
                                <p class="title"><nuxt-link to="/trabajos">Trabajos</nuxt-link></p>
                                <p class="subtitle">+ 100 Trabajos</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 col-lg-4">
                        <div class="congress-content">
                            <img src="~/assets/img/content/simposio.jpg" alt="">
                            <div class="details">
                                <p class="title">Simposio</p>
                                <p class="subtitle">Actualidades en cáncer de mama</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 col-lg-4">
                        <div class="congress-content">
                            <img src="~/assets/img/content/cursos.jpg" alt="">
                            <div class="details">
                                <p class="title"><nuxt-link to="/cursos">Cursos</nuxt-link></p>
                                <p class="subtitle">Lo mejor de las disciplinas en AMM</p>
                            </div>
                        </div>
                    </div-->
                </div>
            </div>
        </section>
        <b-modal id="dudas"  class="text-center" hide-footer>
            <h2 class="text-center">ATENCIÓN DE DUDAS</h2>
            <p class="my-4 text-center">Si tienes dudas generales sobre respecto al congreso, <br>
            escribenos y nos pondremos en contacto a través del correo <br>
            eléctronico que nos proporciones.</p>
            <p class="text-center">Linea de atención a dudas: </p>
            <div class="p-4">
                <b-form @submit.prevent="sendMessage('doubts')" >
                    <b-form-group label="Nombre (s)" label-for="input-nombre">
                        <b-form-input type="text" required v-model="message.name" ></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Paterno" label-for="input-apellido-p">
                        <b-form-input type="text" required v-model="message.last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Materno" label-for="input-apellido-m">
                        <b-form-input type="text" required v-model="message.mother_last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Email" label-for="input-email">
                        <b-form-input type="email" required v-model="message.email"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Duda o problématica" label-for="input-duda">
                        <b-form-textarea type="text" required v-model="message.message"></b-form-textarea>
                    </b-form-group>
                    <b-button variant="primary" class="float-right" type="submit" :disabled="disabled">Enviar</b-button>
                </b-form>
            </div>
        </b-modal>

        <b-modal id="acceso"  class="text-center" hide-footer>
            <h2 class="text-center">PROBLEMAS DE ACCESO</h2>
            <p class="my-4 text-center">Si tienes dudas generales sobre respecto al congreso, <br>
            escribenos y nos pondremos en contacto a través del correo <br>
            eléctronico que nos proporciones.</p>
             <p class="text-center">Linea de atención telefónica: <a class="text-black" style="color:black!important" href="tel:5591638378">55 916 383 78</a> y <a class="text-black" style="color:black!important" href="tel:9841330675">98 413 306 75</a>  </p>
            <div class="p-4">
                <b-form @submit.prevent="sendMessage('access')" >
                    <b-form-group label="Nombre (s)" label-for="input-nombre">
                        <b-form-input type="text" required v-model="message.name" ></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Paterno" label-for="input-apellido-p">
                        <b-form-input type="text" required v-model="message.last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Materno" label-for="input-apellido-m">
                        <b-form-input type="text" required v-model="message.mother_last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Email" label-for="input-email">
                        <b-form-input type="email" required v-model="message.email"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Duda o problématica" label-for="input-duda">
                        <b-form-textarea type="text" required v-model="message.message"></b-form-textarea>
                    </b-form-group>
                    <b-button variant="primary" class="float-right" type="submit" :disabled="disabled">Enviar</b-button>
                </b-form>
            </div>
        </b-modal>

        <b-modal id="pagos"  class="text-center" hide-footer>
            <h2 class="text-center">ACLARACIÓN DE PAGOS</h2>
            <p class="my-4 text-center">Descríbanos el problema sobre el pago de su registro y nos <br>
            pondremos en contacto a través del correo eléctronico que nos <br>
            proporcione</p>
           <!--<p class="text-center">Linea de atención a acalración de pagos: </p>-->
            <div class="p-4">
                <b-form @submit.prevent="sendMessage('payments')" >
                    <b-form-group label="Nombre (s)" label-for="input-nombre">
                        <b-form-input type="text" required v-model="message.name" ></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Paterno" label-for="input-apellido-p">
                        <b-form-input type="text" required v-model="message.last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Materno" label-for="input-apellido-m">
                        <b-form-input type="text" required v-model="message.mother_last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Email" label-for="input-email">
                        <b-form-input type="email" required v-model="message.email"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Duda o problématica" label-for="input-duda">
                        <b-form-textarea type="text" required v-model="message.message"></b-form-textarea>
                    </b-form-group>
                    <b-button variant="primary" class="float-right" type="submit" :disabled="disabled">Enviar</b-button>
                </b-form>

            </div>
        </b-modal>

        <b-modal id="oncologia"  class="text-center" hide-footer>
            <h2 class="text-center">REGISTRO</h2>
            <p class="my-4 text-center">Registra tus datos y recibirás vía correo electrónico una <strong>clave <br>
            de acceso</strong> con la que podrás ingresar de forma gratuita al <br>
            Curso Interdisciplinar de Congreso</p>
            <div class="p-4">
                <b-form @submit.prevent="registerUser()" >
                    <b-form-group label="Nombre (s)" label-for="input-nombre">
                        <b-form-input type="text" required v-model="message.name" ></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Paterno" label-for="input-apellido-p">
                        <b-form-input type="text" required v-model="message.last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Apellido Materno" label-for="input-apellido-m">
                        <b-form-input type="text" required v-model="message.mother_last_name"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Ciudad" label-for="input-duda">
                        <b-form-input type="text" required v-model="message.city"></b-form-input>
                    </b-form-group>
                    <b-form-group label="Email" label-for="input-email">
                        <b-form-input type="email" required v-model="message.email"></b-form-input>
                    </b-form-group>
                    <!--div class="form-group">
                      <label>Especialidad</label>
                      <select class="form-control" required v-model="message.speciality">
                        <option v-for="(speciality, index) in specialities" :key="index" :value="speciality.id">{{ speciality.especialidad }}</option>
                      </select>
                    </div-->

                    <b-button variant="primary" class="float-right" type="submit" :disabled="disabled">Enviar</b-button>
                </b-form>

            </div>
        </b-modal>
        <!-- Blog Area End -->
        <!--<section class="work-company section-padding mt-4" v-if="sponsors.length">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-md-12">
                        Section Tittle
                        <div class="section-tittle section-tittle2 mb-50">
                            <h2 class="text-center">PATROCINADORES OFICIALES DEL CONGRESO</h2>
                        </div>
                    </div>
                    <div class="col-md-12">
                        <client-only>
                            <carousel :loop="true" :per-page="sponsorsCount" :autoplay="true" :paginationEnabled="true" :navigation-enabled="true" paginationActiveColor="#686bc4">
                                <slide v-for="sponsor in sponsors" :key="sponsor.id">
                                    <image-component :picture="sponsor.picture" class="px-3"/>
                                </slide>
                            </carousel>
                        </client-only>
                    </div>
                </div>
            </div>
        </section>-->
        <!--? Brand Area Start-->
        <!--section class="row my-5">
                <div class="col-md-8 offset-md-2">
                    <div class="embed-responsive embed-responsive-16by9">
                        <a class="btn btn-video" href="https://mastologia.org.mx" target="_blank">#VisitMexico</a>
                        <video class="embed-responsive-item"
                               src="~/assets/video/congreso.mp4"
                               loop controls playsinline autoplay muted></video>

                    </div>
                </div>
        </section-->
        <!-- Brand Area End-->
    </main>


</template>

<script>

  import {mapState} from 'vuex';
  import SpeakerComponent from "../components/SpeakerComponent";
  import ImageComponent from "../components/ImageComponent";

  export default {

    middleware: ['guest'],

    components: {ImageComponent, SpeakerComponent},
    data() {
      return {
        sponsors: [],
        sponsorsCount: this.$device.isMobile ? 2 : 4,
        isMobile: this.$device.isMobile,
        loaded: false,
        disabled: false,
        message: {
            name: "",
            last_name: "",
            mother_last_name: "",
            email: "",
            phone_number: "",
            message: "",
            city: "",
            //category: 6,
            //speciality: null
        },
      }
    },
    async mounted() {
      try {
        this.sponsors = await this.$axios.$get(`/sponsors?active_eq=true`);
        this.loaded = true;
      } catch (e) {
        console.warn(e);
        this.$swal('Error', 'Error al obtener profesores', 'error');
      }
    },
    methods: {
       showModal() {
        this.$refs['inicio'].show()
      },
        async sendMessage(type) {

          switch(type){
            case 'doubts':
                  this.message.mail_to = 'atencion@srcongress.mx';
                  break;
            case 'access':
                  this.message.mail_to = 'atencion@srcongress.mx';
                  break;
            case 'payments':
                  this.message.mail_to = 'atencion@srcongress.mx';
                  break;
            default:
                  this.message.mail_to = 'atencion@srcongress.mx';
                  break;
          }

        this.disabled = true;
        this.message.type = type;
        try {
          await this.$axiosAuth.post('/mail/contact', this.message);

          this.$swal('¡Mensaje enviado correctamente!', 'Nos pondremos en contacto contigo a la brevedad.', 'success')
          this.disabled = false;
          this.message = {};
        } catch (e) {
          console.error(e.responseText);
          this.disabled = false;
          this.$swal('¡Error al enviar datos!', 'Por favor contacte directamente a atencion@srcongress.mx', 'error');
        }
      },


        async registerUser() {
          this.disabled = true;
          try {
              let user = await this.$axiosAuth.post(`/auth/register`, {...this.message});
              this.$swal('Registro exitoso.', 'Tu código de acceso se ha enviado correctamente. La recepción puede demorar hasta 5 minutos.', 'success');
              this.disabled = false;
          } catch (e) {
              console.error(e.response);
              this.disabled = false;
              this.$swal('Error',e.response.data.message, 'error');
          }
        },

        openPaymentChat() {
            window.open("/payment-chat", "Chat Aclaración de Pagos");
        }
    },


    computed: {
      ...mapState([
        'event'
      ]),

      countDown() {
        let time = this.$moment(this.event.start_date).valueOf() - this.$moment().startOf('day').valueOf();

        return time < 0 ? 0 : time;
      }
    }

  }
</script>

<style lang="scss" scoped>
    @import "assets/scss/color";
    @import "assets/scss/variables";

    @media (min-width: 1200px) {
        .video-player {
            height: 500px;
        }

        .slider-bg {
            /deep/ .VueCarousel .slider-info {
                padding: 0 10rem !important;

                h1, h2, h3 {
                    font-size: 2.5rem !important;
                }

                img {
                    width: 300px !important;
                }
            }
        }
    }

    .counter-section {
        > h1 {
            color: #FFF;
            font-size: 25px;
            text-align: center;
        }

        position: unset !important;
        font-family: "alegreya-sans-cs", sans-serif;
        background-color: none;
        padding: 25px 25px !important;
        margin: auto;
        border-radius: 10px;
        color: #FFF !important;
        background:#B4215F;
        width: 76%;
        display: block;

        p, span {
            color: #FFF !important;
        }

        .cd-item {
            &:after {
                background: #FFF !important;
                margin-top: 35px;
            }

            &:before {
                background: #FFF !important;
            }

            span {
                margin-top: 20px !important;
                margin-bottom: 0 !important;
            }
        }
    }

    .single-slider {
        background-image: url("/img/banner.jpg");
        background-size: cover !important;
        background-position: top !important;
        background-repeat: no-repeat !important;
        background-attachment: fixed;
    }

    .gradient-bg {
        background-image: linear-gradient(180deg,#516ab7 0%,#37bbe1 100%)!important;
    }

    .team-area {

        .info {
            h2 {
                font-size: 44px;
            }
        }

        .register {
            a {
                display: block;
                margin: 50px auto;
                width: 200px;
            }
        }
    }


    .congress-content {
        margin-bottom: 100px;
        position: relative;

        img {
            z-index: 5;
            position:relative;
            width: 100%;
            -webkit-box-shadow: 0px 0px 10px 1px rgba(0, 0, 0, 0.75);
            -moz-box-shadow: 0px 0px 10px 1px rgba(0, 0, 0, 0.75);
            box-shadow: 0px 0px 10px 1px rgba(0, 0, 0, 0.75);
            min-height: 265px;
        }

        .details {
            position: absolute;
            top: 0;
            width: 100%;
            z-index: 9;
            background-color: #0F6B82;
            left: 0;
            z-index: 1;
            bottom: 0;
            padding: 160px 14px;

            .title {
                text-align: center;
                font-weight: 300;
                font-size: 1.4rem;
                font-family: bebas-neue-pro, sans-serif!important;
                color: #FFF;
                text-shadow: 0px 0px 20px #000000;
                position: absolute;
                bottom: 0;
            }

            .subtitle {
                text-align: center;
                font-weight: 300;
                color: #FFF;
                text-shadow: 0px 0px 20px #000000;
            }
        }

    }

    .video-player {
        width: 100%;

        video {
            width: 100%;
        }
    }

    .slider-bg {
        /deep/ .VueCarousel {
            max-height: 600px;

            .VueCarousel-inner {
                height: 600px !important;
            }

            .VueCarousel-pagination {
                position: absolute;
                bottom: 10px;
            }

            .VueCarousel-slide {
                height: 100%;
            }

            .slider-info {
                width: 100%;
                position: absolute;
                top: 10%;
                padding: 0 1rem;
                text-align: right;

                span, h1, h2, h3 {
                    color: #FFF;
                    text-shadow: 0px 0px 20px #000000;
                    text-transform: uppercase;
                }

                h1 {
                    font-weight: 700 !important;
                    font-size: 26px;
                }

                h2 {
                    font-weight: 700 !important;
                    font-size: 30px !important;
                }

                h3 {
                    font-weight: 700 !important;
                    font-size: 26px;
                }

                img {
                    margin: 25px 0 25px auto !important;
                    width: 170px;
                }
            }
        }
    }

    .VueCarousel-slide > img {
        width: 100%;
        padding-left: 0;
        padding-right: 0;
        height: 100%;
        overflow: hidden;
        object-fit: cover;
    }

    .btn-video {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .work-company {
        background-color: #CFDBE0;

        h2 {
            color: #676bc4!important;
            font-size: 2em;
            letter-spacing:2px;
        }
    }

    @-webkit-keyframes floatText {
        from {
            left: 00%;
        }

        to {
            /* left: auto; */
            left: 100%;
        }
    }
</style>
