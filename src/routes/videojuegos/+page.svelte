<script>
    import Desplegable from "../../lib/desplegable.svelte";
    import IconoPersonalizable from "../../lib/iconoPersonalizable.svelte";
</script>

<main>
    <header class="d-flex flex-column justify-content-center align-items-center">
        <h1>Curso especializado en desarrollo de videojuegos y realidad virtual</h1>
    </header>
    <div class="container"> 
        <section class="iconos d-flex flex-row justify-content-center">
            <IconoPersonalizable
                src = "/src/img/iconosTarjetas/icon_nivel.png"
                alt = "icono-nivel"
                title = "Nivel:"
                texto = "Curso de especialización"

            />
            <IconoPersonalizable
                src = "/src/img/iconosTarjetas/icon_titulo.png"
                alt ="icono-titulo"
                title = "Título:"
                texto = "Desarrollo de videojuegos y realidad virtual"
            />
            <IconoPersonalizable
                src = "/src/img/iconosTarjetas/icon_familia.png"
                alt ="icono-familia"
                title = "Familia Profesional:"
                texto = "Informática y comunicaciones"
            />
        </section>
        <section class="descripcion d-flex flex-column justify-content-center align-items-center">
            <h3>COMPETENCIAS GENERALES DEL CURSO</h3>
            <p> 
                Este curso de especialización permitirá al alumno diseñar y desarrollar videojuegos para diferentes dispositivos
                y plataformas, garantizando la experiencia del usuario, utilizando herramientas de última generación que permitan 
                actuar en todas las fases de su desarrollo, así como aplicaciones interactivas de realidad virtual y aumentada.
            </p>
        </section>
        <section class="salidas-profesionales d-flex flex-column justify-content-center align-items-center">
            <h3>SALIDAS PROFESIONALES</h3>
            <div class="contenido-flex d-flex flex-row justify-content-between align-items-center">
                <img src="/src/img/img_videojuegos.png" alt="videojuegos"/>
                <div class="text-content">
                    <p> La obtención del certificado de este curso de especialización permite ejercer su actividad en empresas, públicas y privadas del sector de los videojuegos, 
                        así como crear su propio estudio de desarrollo de videojuegos.
                    </p>
                    <h6>OCUPACIONES Y PUESTOS RELEVANTES</h6>
                    <ul>
                        <li>Desarrollador de videojuegos</li>
                        <li>Responsable de pruebas de videojuegos</li>
                        <li>Responsable del proceso de creación de videojuegos</li>
                        <li>Diseñador gráfico 2D y 3D de videojuegos</li>
                        <li>Desarrollador de aplicaciones de realidad virtual, aumentada y mixta</li>
                    </ul>
                </div>
            </div>
        </section>
        <section class="acceso d-flex flex-column justify-content-center align-items-center">
            <h3>ACCESO AL CURSO</h3>
            <Desplegable/>
        </section>
        <section class="asignaturas d-flex flex-column justify-content-center align-items-center">
            <h3>CONTENIDO DEL CURSO</h3>
            <table>
                <thead>
                   <td>MÓDULOS PROFESIONALES</td> 
                   <td class="center">HORAS ANUALES</td>
                   <td class="center">HORAS SEMANALES</td>
                </thead>
                <tbody>
                    <tr>
                        <td>5048. Programación y motores de videojuegos.</td>
                        <td class="center">160</td>
                        <td class="center">5</td>
                    </tr>
                    <tr>
                        <td>5049. Diseño gráfico 2D y 3D.</td>
                        <td class="center">125</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td>5050. Programación en red e inteligencia artificial.</td>
                        <td class="center">95</td>
                        <td class="center">3</td>
                    </tr>
                    <tr>
                        <td>5051. Realidad virtual y realidad aumentada.</td>
                        <td class="center">95</td>
                        <td class="center">3</td>
                    </tr>
                    <tr>
                        <td>5052. Diseño, Gestión, publicación y producción</td>
                        <td class="center">125</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td class="der"><strong>Total horas</strong></td>
                        <td class="center"><strong>600</strong></td>
                        <td class="center"><strong>19</strong></td>
                    </tr>
                </tbody>
            </table>
        </section>
    </div>

</main>

<style lang="sass">
    header
        margin: 2rem 0 
        width: 100%
        height: 30rem
        --opacidad-negro: 0.35
        background-image:  linear-gradient(rgba(0, 0, 0, var(--opacidad-negro)), rgba(0, 0, 0, var(--opacidad-negro))), url("/src/img/cabecera_videojuegos.png")
        h1
            color: #FFF
            text-align: center
            font-weight: 600
            font-size: 3rem
    .container
        width: 100%
        h3
            color: #009CDE
            margin: 1rem
        .iconos
            margin: 3rem 0
            gap: 2rem
        .salidas-profesionales
            .contenido-flex
                gap: 5rem
                img 
                    width: 40%
                h6 
                    color:#005D9D
        .acceso 
            width: 100%                
        .asignaturas
            table
                margin: 2rem 0
                width:80%
                thead
                    color: #005D9D
                .center
                    text-align: center
                .der
                    text-align: right    
                tbody
                    tr
                        height: 2.5rem
                        td
                            border-bottom: 0.1rem solid #005D9D
                       
</style>