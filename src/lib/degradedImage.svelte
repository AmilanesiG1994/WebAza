<script>
    export let src, alt, ttr, title, href;
</script>

<main style="--direction:{ttr === 'true' ?'90deg':'270deg'}">
    <div class="container">
        <div class="container-image d-flex {ttr === 'true' ?'flex-row':'flex-row-reverse'}">
            <img {src} {alt}/>
            <div class="gradient"></div>
            <div class ="content d-flex flex-column justify-content-center align-items-center" style="{ttr ? 'right:10%' : 'left:10%'}">
                <div class="titulo"><h3>{title}</h3></div>
                <button class="boton d-flex flex-column align-items-center">
                    <a {href}>VER MÁS</a>
                </button>
            </div>
        </div>
    </div>

</main>

<style lang="sass">
    .container
        margin: 2rem 0
        position: relative
        display: inline-block

        .toLeft
            .content
                order: -1
            img
                order: 1

        .toRight
            .content
                order: 1
            img
                order:1
            
        .gradient
            position: absolute
            width: 20%
            height: 100%
            background: linear-gradient(var(--direction), rgba(255,255,255,0), rgba(255,255,255,0.5), rgba(255,255,255,1))
            top: 0
            left: 40%
            z-index: 200
        
        img
            height: 25rem
            width:60%
        .content
            font-family: Open sans, sans-serif
            width: 40%
            background-color: #FFF
            .titulo
                font-weight: 300
                font-size: 2rem
                line-height: 2.75rem
                text-align: center
                letter-spacing: 0.025em
                //color: #009cde
                color: var(--color)
            .boton
                width: 10rem
                border-radius: 5.5px
                background-color: #005D9D
                height: 3rem
                a
                    padding-top: 0.5rem
                    color: #FFFFFF
                    font-weight: 800
                    letter-spacing: 0.025em
                    text-decoration: none        
</style>