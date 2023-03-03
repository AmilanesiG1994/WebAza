<script>
    import DegradedImage from "../lib/degradedImage.svelte";
</script>

<main>
    <div class="container ">
        <DegradedImage
            src = "/src/img/home_videojuegos.png"
            alt = "CursoVideojuegos"
            ttr = true
            color = white
            title = "Curso especializado en desarrollo de videojuegos y realidad virtual."
            href = "/videojuegos"
        />
        <div class="container">
            <DegradedImage
                src = "/src/img/home_ciberseguridad.png"
                alt = "Ciberseguridad"
                ttr = false
                color = white
                title = "Curso especializado en ciberseguridad."
                href = "/ciberseguridad"
            />
    </div>
   
    
    
</main>

<style lang="sass">
    .container
        width: 100%

</style>