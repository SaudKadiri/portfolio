<div class="card">
    <slot></slot>
</div>

<style>
    .card {
      background-image: linear-gradient(to right bottom, #00091f, #0b0418, #0e010f, #0a0005, #000000);
      background-image: linear-gradient(to left bottom, #333537, #28292b, #1e1d1e, #131212, #000000);
      
      color: #fff;
      border-radius: 15px;
      padding: 40px 50px;
      margin: 20px 0;
      position: relative;
      text-align: center;
    }

    .card:hover {
      box-shadow: 0 0 24px tan;
      background-image: linear-gradient(to right top, #303030, #252525, #1b1b1b, #111111, #000000);
      background-image: linear-gradient(to right bottom, #00091f, #0b0418, #0e010f, #0a0005, #000000);
      /* background-image: linear-gradient(to right bottom, #002707, #1c1c00, #201100, #180702, #000000); */
      color:tan;
    }
  </style>