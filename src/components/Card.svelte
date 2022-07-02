<div class="card">
    <slot></slot>
</div>

<style>
    .card {
      background-image: linear-gradient(to right bottom, #00091f, #0b0418, #0e010f, #0a0005, #000000);
      color: white;
      border-radius: 15px;
      padding: 40px 50px;
      margin: 20px 0;
      position: relative;
      text-align: center;
    }

    .card:hover {
      box-shadow: 0 0 24px tan;
      background-image: linear-gradient(to right top, #000000, #0b0206, #11050f, #140916, #140d1d, #120e1f, #0f1021, #0b1123, #080f20, #060d1d, #030b19, #000816);

      color:tan;
    }
  </style>