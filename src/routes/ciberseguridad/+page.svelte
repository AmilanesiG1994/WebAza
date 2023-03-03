<script>
    import Desplegable from "../../lib/desplegable.svelte";
    import IconoPersonalizable from "../../lib/iconoPersonalizable.svelte";
</script>

<main>
    <header class="d-flex flex-column justify-content-center align-items-center">
        <h1>Curso especializado en ciberseguridad</h1>
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
                Mediante este curso especializado en ciberseguridad adquirirás los conocimientos necesarios para encargarte de la protección 
                de los sistemas de información y redes de comunicaciones, implementando estrategias de seguridad en los sistemas de información 
                realizando diagnósticos de ciberseguridad, identificando vulnerabilidades e implementando las medidas necesarias para mitigarlas 
                aplicando la normativa vigente y estándares del sector.
            </p>
        </section>
        <section class="salidas-profesionales d-flex flex-column justify-content-center align-items-center">
            <h3>SALIDAS PROFESIONALES</h3>
            <div class="contenido-flex d-flex flex-row justify-content-between align-items-center">
                <img src="/src/img/img_ciberseguridad.png" alt="ciberseguridad"/>
                <div class="text-content">
                    <p> 
                        La obtención del certificado de este curso de especialización permite ejercer su actividad en empresas, públicas y privadas del sector 
                        de las telecomunicaciones, finanzas y banca,  servicios informáticos y empresas relacionadas.
                    </p>
                    <h6>OCUPACIONES Y PUESTOS RELEVANTES</h6>
                    <ul>
                        <li>Experto/a en ciberseguridad</li>
                        <li>Auditor/a de ciberseguridad</li>
                        <li>Consultor/a de ciberseguridad</li>
                        <li>Hacker ético</li>
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
                        <td>5021. Incidentes de ciberseguridad</td>
                        <td class="center">120</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td>5022. Bastionado de redes y sistemas</td>
                        <td class="center">210</td>
                        <td class="center">7</td>
                    </tr>
                    <tr>
                        <td>5023. Puesta en producción segura</td>
                        <td class="center">120</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td>5024. Análisis forense informático</td>
                        <td class="center">120</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td>5025. Hacking ético</td>
                        <td class="center">120</td>
                        <td class="center">4</td>
                    </tr>
                    <tr>
                        <td>5026. Normativa de ciberseguridad</td>
                        <td class="center">30</td>
                        <td class="center">1</td>
                    </tr>
                    <tr>
                        <td class="der"><strong>Total horas</strong></td>
                        <td class="center"><strong>720</strong></td>
                        <td class="center"><strong>24</strong></td>
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
        background-image:  linear-gradient(rgba(0, 0, 0, var(--opacidad-negro)), rgba(0, 0, 0, var(--opacidad-negro))), url("/src/img/cabecera_ciberseguridad.png")
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