<script>
    export let src, alt, title, texto;
</script>

<main>
    <div class="content d-flex flex-column justify-content-center align-items-center">
      <img {src} {alt}/>
      <div class="text-area d-flex flex-column align-items-center">
        <h5><strong>{title}</strong></h5> 
        <p>{texto}</p>
      </div> 
    
    </div>
</main>

<style lang="sass">
  main
    flex-basis: 0
    flex-grow: 1
    flex-shrink: 1
    .content
      background-color: #F5F5F5
      border-radius: 0.5rem
      height: 100%
      img 
        padding-top: 1rem
      .text-area
        width:70%
        text-align: center
</style>