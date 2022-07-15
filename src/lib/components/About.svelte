<script>
    import saud_potrait from './../../assets/saud_potrait.jpeg'
    import saud_landscape from './../../assets/saud_landscape.jpg'
</script>
<style>
    img {
        border-radius: 10px;
        width: 100%;
        height: 100%;
    }
    .container {
        margin: auto;
        position: relative;
        width: 100%;
        padding: 0;
    }
    .overlay {
        border-radius: 10px;
        opacity: 0;
    }
    .container:hover .overlay {
        opacity: 0.5;
    }
    .overlay {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        height: 100%;
        width: 100%;
        opacity: 0;
        transition: .5s ease;
        background-image: linear-gradient(to bottom, #d16b6b, #d15978, #ca4a8b, #b744a3, #9348bd, #7a46c3, #5945c9, #1546cf, #1c39c6, #222bbc, #271bb2, #2c00a8);    
    }
    .text {
        color:white;
        font-size: 20px;
        position: absolute;
        top: 50%;
        left: 50%;
        -webkit-transform: translate(-50%, -50%);
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        text-align: center;
    }
</style>
<div class="container">
    <picture>
        <source 
           media="(orientation: landscape)"
           srcset={saud_landscape}>
        <source 
           media="(orientation: portrait)"
           srcset={saud_potrait}>   
        <img src={saud_potrait} alt="Saud's selfie at his favorite place-Dnyandeep College." height="250px" />
    </picture>
    <div class="overlay">
        <p class="text" style="font-size:2.1vmin">This is a selfie from my last visit to my favorite place- Dnyandeep School. A place that lasts forever in my heart.</p>
    </div>
</div>
