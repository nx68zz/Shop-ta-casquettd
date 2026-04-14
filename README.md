# Shop-ta-casquette
Boutique de casquette en ligne 
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shop ta casquette</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<header>
🧢 Shop ta casquette
</header>

<div class="container">

<div class="product">
<img src="https://via.placeholder.com/400x300" alt="Casquette">
<h2>Casquette Street Style</h2>
<p>Casquette stylée et confortable 🔥</p>
<p class="price">29,99 €</p>

<button onclick="addToCart()">Ajouter au panier</button>
</div>

<div class="cart">
<h3>🛒 Panier</h3>
<p id="cartText">Ton panier est vide</p>
<p id="total"></p>

<button onclick="checkout()">Commander</button>
</div>

</div>

<footer>
© 2026 Shop ta casquette
</footer>

<script>
let cart = 0;

function addToCart() {
    cart = 29.99;
    document.getElementById("cartText").innerText = "1 casquette ajoutée 🧢";
    document.getElementById("total").innerText = "Total : " + cart + " €";
}

function checkout() {
    if(cart > 0){
        alert("Commande envoyée (demo) 🧢");
    } else {
        alert("Ton panier est vide !");
    }
}
</script>

</body>
</html>
