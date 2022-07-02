<script>
    export let src
</script>
<style>
    img {
        border-radius: 10px;
        width: 100%;
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
    <img {src} alt="Saud's selfie at his favorite place-Dnyandeep College." height="250px"/>
    <div class="overlay">
        <p class="text">This is my last selfie from my favorite place- Dnyandeep School. A place that lasts forever in my heart.</p>
    </div>
</div>
