<div class="card">
    <slot></slot>
</div>

<style>
    .card {
      background-color: #fff;
      color: #333;
      border-radius: 15px;
      padding: 40px 50px;
      margin: 20px 0;
      position: relative;
      text-align: center;
    }

    .card:hover {
      box-shadow: 0 0 24px lavender;
      background-color: black;
      color: white;
    }
  </style>