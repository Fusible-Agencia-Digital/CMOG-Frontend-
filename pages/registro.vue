<template>
    <main>
        <!--? Hero Start -->
        <div class="slider-area2">
            <div class="slider-height2 d-flex align-items-center">
                <div class="container">
                    <div class="row">
                        <div class="col-xl-12">
                            <div class="hero-cap text-center">
                                <h2>Registro</h2>
                                <h4 class="text-white">Información importante sobre el registro</h4>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <menu-tabs-component>
                <!--<b-nav-item :active="activeTab===0" @click="activeTab=0" href="#"
                            v-scroll-to="{el: '#general', offset: -180}">Información general
                </b-nav-item>-->
                <b-nav-item :active="activeTab===1" @click="activeTab=1" href="#"
                            v-scroll-to="{el: '#costo', offset: -180}">Costos
                </b-nav-item>
                <!--<b-nav-item :active="activeTab===2" @click="activeTab=2" href="#"
                            v-scroll-to="{el: '#grupales', offset: -180}">Inscripciones grupales
                </b-nav-item>-->
                <!--<b-nav-item :active="activeTab===3" @click="activeTab=3" href="#"
                            v-scroll-to="{el: '#limite', offset: -180}">Límite de inscripción
                </b-nav-item>-->
                <b-nav-item :active="activeTab===4" @click="activeTab=4" href="#"
                            v-scroll-to="{el: '#formas', offset: -180}">Formas de pago
                </b-nav-item>
                <!--<b-nav-item :active="activeTab===5" @click="activeTab=5" href="#"
                            v-scroll-to="{el: '#politica', offset: -180}">Políticas de cancelación
                </b-nav-item>-->
                <!--<b-nav-item href="https://www.mastologia.org.mx/registro/carta/solicitud.php" target="_blank">Carta
                    Permiso
                </b-nav-item>-->
            </menu-tabs-component>
        </div>
        <!-- Hero End -->
        <!--? Brand Area Start -->
        <section class="team-area pb-100">
            <div class="container">
                <div class="row">
                    <div class="col-md-12">
                        <!--<div class="card card-info" id="general">
                            <div class="card-header">
                                <h2 class="mb-0">Información importante sobre el Registro</h2>
                            </div>
                            <div class="card-body">
                                <p>Tenga en cuenta que para 2020 tenemos nuevos requisitos en torno al <em>Congreso
                                    Virtual</em>. Se requiere una dirección de correo electrónico única para cada
                                    individuo para acceder a la plataforma virtual. Sin una dirección de correo
                                    electrónico única, el miembro del grupo no podrá obtener acceso al Congreso virtual.
                                </p>
                                <p><span style="font-size: 19px;">Esta dirección de correo electrónico también se utilizará para enviar cualquier correspondencia relevante y acceder a la constancia después del congreso. Proporcionar esta información por adelantado también nos permitirá procesar todos los registros individuales o de grupo de manera eficiente y entregar detalles de inicio de sesión a los registrados de manera oportuna.</span>
                                </p>
                            </div>
                        </div>-->

                        <div class="card card-info" id="costo">
                            <div class="card-header">
                                <h2 class="mb-0">Costos durante el congreso</h2>
                            </div>
                            <div class="card-body">
                                <div class="row title-cost">
                                    <div class="col">
                                        <h3>Registro Individual</h3>
                                        <div class="card mb-4 mt-md-4">
                                            <h5 class="card-header">Especialistas</h5>
                                            <div class="card-body">
                                                <h6 class="card-title">Inscripción al Congreso Nacional $3,000.00</h6>
                                                <h6>Anualidad 2020 $2,000.00</h6>
                                                <h6>Inscripción al Colegio $2,000.00</h6>
                                            </div>
                                        </div>
                                        <div class="card mb-4">
                                            <h5 class="card-header">Residentes, estudiantes y personal paramédico</h5>
                                            <div class="card-body">
                                                <h6 class="card-title">Inscripción al congreso $ 1,500.00</h6>
                                            </div>
                                        </div>
                                        <div class="card">
                                            <h5 class="card-header">Extranjeros</h5>
                                            <div class="card-body">
                                                <h6 class="card-title">Inscripción al congreso 150 dlls</h6>
                                            </div>
                                        </div>
                                        <a href="https://www.srcongress.mx/cmog/registro_virtual.php"
                                           target="_blank" class="btn w-100 mb-5 mb-md-3 mt-3">
                                            Registro individual
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>



                        <!--<div class="card card-info" id="limite">
                            <div class="card-header">
                                <h2 class="mb-0">Fecha límite de inscripción</h2>
                            </div>
                            <div class="card-body">
                                <p>El último día para recibir el pago del descuento de la tarifa anticipada es de 21 de
                                    agosto de 2020.</p>
                                <p>El día 30 de Septiembre el registro en línea se cerrará, por lo que deberá realizar
                                    su inscripción en línea hasta el día del congreso, esto puede demorar en las
                                    validaciones por lo que le sugerimos inscribirse antes de Septiembre 30.</p>
                            </div>
                        </div>-->

                        <!--<div class="card card-info" id="">
                            <div class="card-header">
                                <h2 class="mb-0">Confirmaciones de pago</h2>
                            </div>
                            <div class="card-body">
                                <p>Las confirmaciones de inscripción son automáticas si son realizadas con tarjeta de
                                    débito ó crédito, las transferencias bancarias si requieren de validación
                                    administrativa.</p>
                            </div>
                        </div>-->


                        <div class="row" id="formas">
                            <div class="col-md-12">
                                <div class="card card-info">
                                    <div class="card-header">
                                        <h2 class="mb-0">Formas de pago</h2>
                                    </div>
                                    <div class="card-body title-cost">
                                        <p>Para su comodidad contamos con las siguientes formas de pago:</p>
                                        <h3>Datos bancarios</h3>
                                       <ul>
                                           <li>HQ Colegio de Oncólogos Ginecólogos AC</li>
                                           <li>BBVA Bancomer</li>
                                           <li>Suc. 1378</li>
                                           <li>No. de Cta: 0115459087</li>
                                           <li>CLABE interbancaria: 012180001154590878</li>
                                       </ul>

                                    </div>
                                </div>
                            </div>
                            <!--<div class="col-md-6">
                                <div class="card card-info">
                                    <div class="card-header">
                                        <h2 class="mb-0">Dudas sobre el registro</h2>
                                    </div>
                                    <div class="card-body">
                                        <p>
                                            <a href="https://www.srcongress.mx/masto/registro/registro_virtual_amm.php"
                                               target="_blank">Regístrese en línea aquí</a></p>
                                        <p>Para consultas o dudas de registro, llame al +52 5555530672 ó 5552116604 </p>
                                        <p>También puede escribirnos a
                                            <a href="mailto:registro@mastologia.org.mx">registro@mastologia.org.mx</a>
                                        </p>
                                    </div>
                                </div>
                            </div>-->
                        </div>


                        <!--<div class="card card-info" id="politica">
                            <div class="card-header">
                                <h2 class="mb-0">Políticas de cancelación</h2>
                            </div>
                            <div class="card-body">
                                <p>Las solicitudes de cancelación para el XVII Congreso Nacional de Mastología deben
                                    recibirse por escrito antes del 31 de agosto de 2020 al correo
                                    <a href="mailto:registro@mastologia.org.mx">registro@mastologia.org.mx</a></p>
                                <p>Todos los rembolsos están sujetos a un cargo del 50% del valor de inscripción. No se
                                    aceptarán cancelaciones por teléfono. Por favor, envíe correo electrónico: <a
                                            href="mailto:registro@mastologia.org.mx">registro@mastologia.org.mx</a></p>
                                <p>Para las tarifas de registro inferiores a $2000.00, la tarifa de registro no es
                                    reembolsable. En lugar de un reembolso, también puede solicitar un cupón para
                                    participar en una reunión futura.</p>
                                <p>Los solicitantes de registro que deseen cancelar pueden transferir su registro a otra
                                    persona sin penalización si envían una solicitud por escrito con el nombre de la
                                    persona de reemplazo antes del 31 de agosto de 2020.</p>
                                <p>Las cancelaciones recibidas después del 31 de agosto de 2020 recibirán un comprobante
                                    de participación en una reunión futura. Si no cancela por adelantado, no se emitirán
                                    reembolsos una vez que el evento haya concluido, independientemente de si participó
                                    en el evento.</p>
                                <p>Se pueden ofrecer vales de crédito si el programa se suspende o acorta debido a
                                    condiciones o circunstancias que escapan al control de comité organizador,
                                    incluidas, entre otras, el clima, interrupciones en los servicios de Internet,
                                    cortes de energía y cualquier cancelación relacionada con la epidemia de
                                    COVID-19.</p>
                            </div>
                        </div>-->


                    </div>
                </div>
            </div>
        </section>
        <!-- Brand Area End -->
    </main>
</template>

<script>
  export default {
    data() {
      return {
        activeTab: 1
      }
    },

    middleware: ['guest'],
  }
</script>

<style lang="scss">
    .slider-area2 {
        background-image: url(/images/cover_main.jpg);
    }

    .nav-link {
        padding-left: 17px !important;
        padding-right: 17px !important;
    }

    .card-info {
        border: 0px;

        .card-header {
            background: none;

            h2 {
                font-size: 18pt;
            }
        }

        .card-body {
            p {
                color: #7f8192;

                a {
                    color: #eb008a;
                }
            }

            ul {
                li {
                    list-style-type: circle;
                    margin-left: 30px;
                    color: #7f8192;

                    a {
                        color: #eb008a;
                    }
                }
            }
        }
    }

    .title-cost {
        h3 {
            color: #B4215F;
            font-size: 20px;
        }
    }
</style>
