<!DOCTYPE html>
<html lang="ka">
<head>
  <meta charset="UTF-8">
  <title>ონლაინ მაღაზია</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f9f9f9;
    }
    header {
      background-color: #333;
      color: white;
      padding: 15px;
      text-align: center;
    }
    .products {
      display: flex;
      justify-content: space-around;
      padding: 20px;
      flex-wrap: wrap;
    }
    .product {
      background: white;
      border: 1px solid #ddd;
      padding: 10px;
      width: 200px;
      margin: 10px;
      text-align: center;
    }
    .product img {
      width: 100%;
      height: auto;
    }
  </style>
</head>
<body>

  <header>
    <h1>ჩემი ონლაინ მაღაზია</h1>
  </header>

  <div class="products">
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="პროდუქტი">
      <h3>პროდუქტი 1</h3>
      <p>₾30.00</p>
      <button>დამატება კალათაში</button>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/200" alt="პროდუქტი">
      <h3>პროდუქტი 2</h3>
      <p>₾45.00</p>
      <button>დამატება კალათაში</button>
    </div>
  </div>

  <!-- აქ დაემატა სკრიპტი -->
  <script>
    const buttons = document.querySelectorAll(".product button");

    buttons.forEach((button) => {
      button.addEventListener("click", () => {
        const product = button.parentElement.querySelector("h3").innerText;
        alert(`პროდუქტი "${product}" დაემატა კალათაში!`);
      });
    });
  </script>

</body>
</html>
