<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
 
    <title>Taller Mecánico MCQueen</title>
    <!-- Enlaces a archivos CSS  -->
    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <!-- Enlaces a archivos JS -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <!-- Estilos personalizados -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#" onclick="mostrarSeccion('inicio')">Taller Mecánico RayoMcQueen</a>
        <!-- boton de navbar -->
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="#" onclick="mostrarSeccion('inicio')">Inicio</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" onclick="mostrarSeccion('servicios')">Servicios</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" onclick="mostrarSeccion('galeria')">Galería</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" onclick="mostrarSeccion('contacto')">Contacto</a>
                </li>
            </ul>
            <!-- Formulario de búsqueda -->
            <form class="form-inline my-2 my-lg-0">
                <input class="form-control mr-sm-2" type="search" placeholder="Buscar" aria-label="Buscar">
                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Buscar</button>
            </form>
        </div>
    </nav>

    <!-- primer div -->
    <div class="container">
        <!-- Página de inicio -->
        <div id="inicio" class="seccion">
            <!-- Logo  -->
            <div class="row">
                <div class="col-md-6">
                    <img src="imagen/descarga.png" alt="Logo del taller" class="img-fluid mt-3 mb-3">
                    <!-- Texto -->
                    <p class="text-muted">Horario de atención: 8:00 am - 19:00 pm</p>
                    <!-- Mapa -->
                    <p>Encuéntranos en Google Maps <a href="https://www.google.com/maps/place/Duoc+UC:+Sede+Vi%C3%B1a+Del+Mar/@-33.0336846,-71.5377975,17z/data=!3m1!4b1!4m6!3m5!1s0x9689de64d74fd4af:0x8004f381e9055a38!8m2!3d-33.0336892!4d-71.5331841!16s%2Fg%2F1v420nzr?entry=ttu">aquí</a>.</p>
                </div>
                <div class="col-md-6">
                    <!-- Rayo McQueen-->
                    <img src="imagen/rayo.png" alt="Rayo McQueen">
                </div>
            </div>
            <!-- Servicios -->
            <br><br>
            <h3><center>Servicios</center></h3>
            <br><br>
            <div class="row">
                <div class="col-md-3">
                    <div class="service-item">
                        <h4>Servicio de Frenos</h4>
                        <img src="imagen/frenos.jpg" alt="Servicio de Frenos">
                        <p>Contamos con el equipamiento necesario para garantizar el correcto funcionamiento de los frenos de su auto. Nuestro equipo de mecánicos altamente capacitados se asegurará de que sus frenos estén en perfectas condiciones para su tranquilidad y seguridad.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-item">
                        <h4>Cambio de Aceite</h4>
                        <img src="imagen/aceite.png" alt="Cambio de Aceite">
                        <p>En Talleres RayoMCQueen nos preocupamos de contar con la mejor calidad en Aceites de Motor y Filtros de Aceites para realizar el cambio necesario y asegurar un buen funcionamiento de su vehículo, a un buen precio.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-item">
                        <h4>Mantenimiento Preventivo</h4>
                        <img src="imagen/mantencion.jfif" alt="Mantenimiento Preventivo">
                        <p>Nuestro compromiso es ofrecer el mejor estándar en calidad de servicio, por eso contamos con un equipo especializado capaz de realizar un mantenimiento multimarca para cualquier tipo de vehículo.</p>
                    </div>
                </div>
            </div>
            <!-- Otros Servicios -->
            <div class="row mt-3">
                <div class="col-md-12">
                    <div class="card">
                        <div class="card-body">
                            <h4 class="card-title">Otros Servicios</h4>
                            <ul class="list-unstyled">
                                <li><a href="#">Mantenimiento de Flotas</a></li>
                                <li><a href="#">Revisión Mecánica</a></li>
                                <li><a href="#">Balanceo de Neumáticos</a></li>
                                <li><a href="#">Kit de Embrague</a></li>
                                <li><a href="#">Sistema Eléctrico</a></li>
                                <li><a href="#">Amortiguadores</a></li>
                                <li><a href="#">Revisión Técnica</a></li>
                                <li><a href="#">Ver Todos</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Carrusel de imágenes -->
            <div id="carouselExampleControls" class="carousel slide mt-5" data-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="imagen/5f1602b8d32e5.jpeg" class="d-block w-100"   alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="imagen/depositphotos_392802712-stock-photo-selective-focus-mechanic-overalls-fixing.jpg" class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="imagen/sss.jpg" class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="imagen/auto-mechanic-640x230.jpg" class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="imagen/images (1).jpg" class="d-block w-100" alt="...">
                    </div>
                </div>
                <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="sr-only">Previous</span>
                </a>
                <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="sr-only">Next</span>
                </a>
            </div>
            <!-- Sección de redes sociales -->
            <div id="redesSociales" class="col-md-12 text-center mt-5">
                <!-- Aquí se mostrarán dinámicamente los enlaces a las redes sociales -->
            </div>
        </div>
        <br><br>
        <!-- Sección de servicios (por defecto oculta) -->
        <div id="servicios" class="seccion" style="display:none;">
            <div class="row mt-5">
                <div class="col-md-6 offset-md-3 text-center">
                    <h2>Servicios</h2>
                    <!-- formulario de servicios -->
                    <form id="formularioServicios">
                        <div class="form-group">
                            <label for="tipo_servicio">Tipo de Servicio</label>
                            <select class="form-control" id="tipo_servicio">
                                <option value="reparacion">Reparación</option>
                                <option value="mantenimiento">Mantenimiento</option>
                                <option value="instalacion">Instalación</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="descripcion">Descripción</label>
                            <textarea class="form-control" id="descripcion" rows="3" required></textarea>
                        </div>
                        <button type="button" class="btn btn-primary" onclick="calcularCosto()">Calcular Costo</button>
                        <div id="costoResultado" style="display: none;">
                            <p>Costo estimado: <span id="costoEstimado"></span></p>
                        </div>
                    </form>
                </div>
            </div>
        </div>

        <!-- Galería  -->
        <div id="galeria" class="seccion" style="display:none;">
            <!-- Galería de imágenes -->
            <div class="collage">
                <img src="imagen/galeria1.jfif" alt="Galería 1">
                <img src="imagen/galeria2.jfif" alt="Galería 2">
                <img src="imagen/galeria3.jfif" alt="Galería 3">
                <img src="imagen/galeria4.jfif" alt="Galería 4">
                <img src="imagen/galeria5.jfif" alt="Galería 5">
                <img src="imagen/galeria6.jfif" alt="Galería 6">
                <img src="imagen/galeria7.jfif" alt="Galería 7">
                <img src="imagen/galeria8.jfif" alt="Galería 8">
                <img src="imagen/galeria9.jfif" alt="Galería 9">
                <img src="imagen/galeria10.jfif" alt="Galería 10">
                <!-- Agrega más imágenes aquí -->
            </div>
        </div>

        <!-- Formulario de contacto (por defecto oculta) -->
        <div id="contacto" class="seccion" style="display:none;">
            <div class="row mt-5">
                <!-- Columna del sistema (sys) -->
                <div class="col-md-6">
                    <div class="card">
                        <div class="card-body">
                            <h5 class="card-title">Comunícate con nosotros</h5>
                            <p class="card-text">Teléfono: +56967329047</p>
                            <p class="card-text">Correo Electrónico: TallerRayoMCQUEEN</p>
                            <a href="https://media.tenor.com/Qb7l9m4NF2sAAAAe/te-la-creiste-we-xd-te-la-kreiste-we-xd.png" class="card-link">Envíanos un Whatsapp</a>
                        </div>
                    </div>
                </div>
                <!-- Columna del formulario (sos) -->
                <div class="col-md-6">
                    <h2>Envíanos un mensaje</h2>
                    <form>
                        <div class="form-group">
                            <label for="nombre">Nombre*</label>
                            <input type="text" class="form-control" id="nombre" placeholder="Nombre" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Correo*</label>
                            <input type="email" class="form-control" id="email" placeholder="Correo Electrónico" required>
                        </div>
                        <div class="form-group">
                            <label for="telefono">Teléfono*</label>
                            <input type="tel" class="form-control" id="telefono" placeholder="Teléfono" required>
                        </div>
                        <div class="form-group">
                            <label for="comuna">Comuna*</label>
                            <input type="text" class="form-control" id="comuna" placeholder="Comuna" required>
                        </div>
                        <div class="form-group">
                            <label for="mensaje">Mensaje</label>
                            <textarea class="form-control" id="mensaje" rows="3"></textarea>
                        </div>
                        <div class="form-check">
                            <input type="checkbox" class="form-check-input" id="politicaPrivacidad" required>
                            <label class="form-check-label" for="politicaPrivacidad">He leído y acepto la política de privacidad.</label>
                        </div>
                        <button type="submit" class="btn btn-primary">Enviar</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <!-- (Pie de página)-->
    <footer class="footer mt-auto py-3">
        <div class="container">
            <span class="text-muted">© 2024 Taller Mecánico RayoMCQueen. Todos los derechos reservados.</span>
        </div>
    </footer>

    <!-- Scripts personalizados -->
    <script src="scripts.js"></script>
    <script>
        // Función 1: Mostrar una sección específica
        function mostrarSeccion(idSeccion) {
            // Ocultar todas las secciones
            $(".seccion").hide();
            // Mostrar la sección correspondiente al ID proporcionado
            $("#" + idSeccion).show();
        }

        // Función 2: Calcular costo del servicio
        function calcularCosto() {
            var tipoServicio = $("#tipo_servicio").val();
            var descripcion = $("#descripcion").val();
            var precio = 0;

            // Asignar un valor por defecto al precio según el tipo de servicio
            switch(tipoServicio) {
                case "reparacion":
                    precio = 100; // Valor por defecto para reparación
                    break;
                case "mantenimiento":
                    precio = 80; // Valor por defecto para mantenimiento
                    break;
                case "instalacion":
                    precio = 120; // Valor por defecto para instalación
                    break;
                default:
                    precio = 0;
            }

            // Calcular el costo final
            var costoFinal = precio * descripcion.length;

            // Mostrar el resultado en la página
            $("#costoEstimado").text("$" + costoFinal);
            $("#costoResultado").show();
        }

        // Función 3: Mostrar enlaces a redes sociales
        function mostrarRedesSociales() {
            // HTML para los enlaces a las redes sociales
            var redesHTML = `
                <h4>Síguenos en nuestras redes sociales</h4>
                <h6>no contamos con un instagram, pero sigue a nuestros amigos!</h6>
                <!-- Agrega tus enlaces a redes sociales aquí -->
                <a href="https://www.facebook.com/TallerMecanicoRayoMcQueen" target="_blank"><img src="imagen/facebook.png" alt="Facebook"></a>
                <a href="https://www.instagram.com/mecanator" target="_blank"><img src="imagen/instagram.png" alt="Instagram"></a>
                <a href="https://twitter.com/RayoMcQueenTaller" target="_blank"><img src="imagen/twitter.png" alt="Twitter"></a>
            `;
            
            // Agregar el HTML al contenedor de redes sociales
            $("#redesSociales").html(redesHTML);
        }

        // Mostrar la página de inicio 
        mostrarSeccion('inicio');
        // Mostrar enlaces a redes sociales
        mostrarRedesSociales();
    </script>
</body>
</html>
