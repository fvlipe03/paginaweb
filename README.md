<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taller Mecánico MCQueen</title>
    <!-- Enlaces a archivos CSS -->
    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <!-- Enlaces a archivos JS -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <!-- Estilos personalizados -->
    <link rel="stylesheet" href="styles.css">

    <!-- Script para el reloj -->
    <script>
        function actualizarReloj() {
            var ahora = new Date();
            var horas = ahora.getHours();
            var minutos = ahora.getMinutes();
            var segundos = ahora.getSeconds();

            // Añadir cero al principio de los números menores de 10
            if (horas < 10) horas = "0" + horas;
            if (minutos < 10) minutos = "0" + minutos;
            if (segundos < 10) segundos = "0" + segundos;

            var horaActual = horas + ":" + minutos + ":" + segundos;
            document.getElementById("reloj").textContent = horaActual;
        }

        // Actualizar el reloj cada segundo
        setInterval(actualizarReloj, 1000);
        // Llamar a la función inmediatamente para mostrar la hora actual sin esperar un segundo
        document.addEventListener("DOMContentLoaded", actualizarReloj);
    </script>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#" onclick="mostrarSeccion('inicio')">Taller Mecánico RayoMcQueen</a>
        <!-- Botón de navbar -->
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

    <!-- Contenido de la página -->
    <div class="container">
        <!-- Página de inicio -->
        <div id="inicio" class="seccion">
            <!-- Logo -->
            <div class="row">
                <div class="col-md-6">
                    <img src="imagen/descarga.png" alt="Logo del taller" class="img-fluid mt-3 mb-3">
                    <!-- Texto -->
                    <p class="text-muted">Horario de atención: 8:00 am - 19:00 pm</p>
                    <!-- Mapa -->
                    <p>Encuéntranos en Google Maps <a href="https://www.google.com/maps/place/Duoc+UC:+Sede+Vi%C3%B1a+Del+Mar/@-33.0336846,-71.5377975,17z/data=!3m1!4b1!4m6!3m5!1s0x9689de64d74fd4af:0x8004f381e9055a38!8m2!3d-33.0336892!4d-71.5331841!16s%2Fg%2F1v420nzr?entry=ttu">aquí</a>.</p>
                    <!-- Reloj -->
                    <p>Hora actual: <span id="reloj"></span></p>
                </div>
                <div class="col-md-6">
                    <!-- Imagen de Rayo McQueen -->
                    <img src="imagen/rayo.png" alt="Rayo McQueen">
                </div>
            </div>

            <!-- Servicios -->
            <h3 class="text-center mt-5">Servicios</h3>
            <div class="row mt-4">
                <div class="col-md-4">
                    <div class="service-item">
                        <h4>Servicio de Frenos</h4>
                        <img src="imagen/frenos.jpg" alt="Servicio de Frenos" class="img-fluid">
                        <p>Contamos con el equipamiento necesario para garantizar el correcto funcionamiento de los frenos de su auto. Nuestro equipo de mecánicos altamente capacitados se asegurará de que sus frenos estén en perfectas condiciones para su tranquilidad y seguridad.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-item">
                        <h4>Cambio de Aceite</h4>
                        <img src="imagen/aceite.png" alt="Cambio de Aceite" class="img-fluid">
                        <p>En Talleres RayoMcQueen nos preocupamos de contar con la mejor calidad en Aceites de Motor y Filtros de Aceites para realizar el cambio necesario y asegurar un buen funcionamiento de su vehículo, a un buen precio.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-item">
                        <h4>Mantenimiento Preventivo</h4>
                        <img src="imagen/mantencion.jpg" alt="Mantenimiento Preventivo" class="img-fluid">
                        <p>Nuestro compromiso es ofrecer el mejor estándar en calidad de servicio, por eso contamos con un equipo especializado capaz de realizar un mantenimiento multimarca para cualquier tipo de vehículo.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <footer class="footer bg-light py-3">
        <div class="container text-center">
            <p class="text-muted">&copy; 2023 Taller Mecánico Rayo McQueen. Todos los derechos reservados.</p>
        </div>
    </footer>
</body>
</html>
