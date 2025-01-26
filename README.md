<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GRODT - Webshop</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f7f7f7;
            color: #333;
        }
        header {
            background: #333;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        .hero {
            background: url('https://via.placeholder.com/1500x500') no-repeat center center/cover;
            height: 300px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }
        .hero h1 {
            font-size: 3rem;
        }
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1rem;
            padding: 2rem;
        }
        .product {
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            padding: 1rem;
        }
        .product img {
            width: 100%;
            height: auto;
        }
        .product h2 {
            font-size: 1.5rem;
            margin: 1rem 0;
        }
        .product p {
            font-size: 1rem;
            color: #666;
        }
        .product button {
            background: #333;
            color: white;
            border: none;
            padding: 0.75rem 1.5rem;
            border-radius: 25px;
            cursor: pointer;
            transition: background 0.3s ease;
        }
        .product button:hover {
            background: #555;
        }
    </style>
</head>
<body>
    <header>
        <h1>GRODT - Get Rich or Die Trying</h1>
    </header>
    <div class="hero">
        <h1>Welkom bij onze webshop</h1>
    </div>
    <section class="products">
        <div class="product">
            <img src="https://via.placeholder.com/300" alt="Product 1">
            <h2>Product 1</h2>
            <p>&euro;49.99</p>
            <button>Koop nu</button>
        </div>
        <div class="product">
            <img src="https://via.placeholder.com/300" alt="Product 2">
            <h2>Product 2</h2>
            <p>&euro;59.99</p>
            <button>Koop nu</button>
        </div>
        <div class="product">
            <img src="https://via.placeholder.com/300" alt="Product 3">
            <h2>Product 3</h2>
            <p>&euro;69.99</p>
            <button>Koop nu</button>
        </div>
    </section>
</body>
</html>
