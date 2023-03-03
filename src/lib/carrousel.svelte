<script>
    export let src1, src2, src3, src4, alt;
</script>

<main>
    <div class="container">
        <div class="wrapper">
            <img src="{src1}" alt="{alt}">
            <img src="{src2}" alt="{alt}">
            <img src="{src3}" alt="{alt}">
            <img src="{src4}" alt="{alt}">
         </div>
    </div>
</main>

<style lang="sass">
    main
        padding: 0
        margin: 0
        box-sizing: border-box
        z-index: -1
        .container
            width: 100%
            position: absolute
            transform: translate(-50%,-50%)
            top: 50%
            left: 50%
            overflow: hidden
            .wrapper
                width: 100%
                display: flex
                animation: slide 16s infinite
                img
                    width: 100% 
                    height: 15rem
@keyframes slide
    0%
        transform: translateX(0)
    25%
        transform: translateX(0)
    30%
        transform: translateX(-100%)
    50%
        transform: translateX(-100%)
    55%
        transform: translateX(-200%)
    75%
        transform: translateX(-200%)
    80%
        transform: translateX(-300%)
    100%
        transform: translateX(-300%)
</style>