
 <!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Las.kys | T-shirts Personnalisés Premium</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  min-height: 100vh;
}

header {
  background: linear-gradient(90deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
  color: white;
  padding: 20px 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-shadow: 0 8px 32px rgba(0,0,0,0.3);
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-left {
  display: flex;
  align-items: center;
  gap: 20px;
  flex: 1;
}

.logo {
  font-size: 28px;
  font-weight: bold;
  background: linear-gradient(45deg, #ff6b6b, #ff8e72, #ffd93d);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.search-box {
  display: flex;
  gap: 10px;
  flex: 1;
  max-width: 400px;
}

.search-box input {
  flex: 1;
  padding: 10px 15px;
  border: none;
  border-radius: 25px;
  background: rgba(255,255,255,0.1);
  color: white;
  border: 2px solid rgba(255,255,255,0.2);
}

.search-box input::placeholder {
  color: rgba(255,255,255,0.6);
}

.search-box input:focus {
  outline: none;
  border-color: #ffd93d;
  background: rgba(255,255,255,0.15);
}

.search-box button {
  padding: 10px 20px;
  background: #ff6b6b;
  border: none;
  border-radius: 25px;
  color: white;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s ease;
}

.search-box button:hover {
  background: #ff8e72;
  transform: scale(1.05);
}

.header-right {
  display: flex;
  gap: 15px;
  align-items: center;
}

.cart-icon {
  background: linear-gradient(45deg, #ff6b6b, #ff8e72);
  color: white;
  padding: 10px 20px;
  border-radius: 25px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s ease;
  border: none;
}

.cart-icon:hover {
  transform: scale(1.08);
  box-shadow: 0 5px 20px rgba(255,107,107,0.4);
}

.track-order-btn {
  background: linear-gradient(45deg, #4facfe, #00f2fe);
  color: white;
  padding: 10px 20px;
  border-radius: 25px;
  cursor: pointer;
  font-weight: bold;
  border: none;
  transition: all 0.3s ease;
}

.track-order-btn:hover {
  transform: scale(1.08);
  box-shadow: 0 5px 20px rgba(79,172,254,0.4);
}

.hero {
  text-align: center;
  padding: 60px 20px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
}

.hero h1 {
  font-size: 48px;
  margin-bottom: 15px;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.hero p {
  font-size: 18px;
  margin-bottom: 20px;
  opacity: 0.9;
}

.hero-features {
  display: flex;
  justify-content: center;
  gap: 30px;
  flex-wrap: wrap;
  margin-top: 20px;
}

.feature {
  background: rgba(255,255,255,0.1);
  padding: 15px 25px;
  border-radius: 15px;
  backdrop-filter: blur(10px);
}

.products {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 25px;
  padding: 40px;
  max-width: 1400px;
  margin: 0 auto;
}

.product {
  background: white;
  padding: 20px;
  border-radius: 15px;
  text-align: center;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
  transition: all 0.3s ease;
  overflow: hidden;
}

.product:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 40px rgba(0,0,0,0.3);
}

.product-image {
  width: 100%;
  height: 250px;
  border-radius: 10px;
  margin-bottom: 15px;
  object-fit: cover;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.product-tag {
  display: inline-block;
  background: linear-gradient(45deg, #ff6b6b, #ff8e72);
  color: white;
  padding: 5px 12px;
  border-radius: 20px;
  font-size: 12px;
  margin-bottom: 10px;
  font-weight: bold;
}

.product h2 {
  margin: 10px 0;
  color: #1a1a2e;
  font-size: 18px;
}

.product-color {
  font-size: 14px;
  color: #666;
  margin: 8px 0;
}

.colors {
  display: flex;
  justify-content: center;
  gap: 8px;
  margin: 10px 0;
}

.color-dot {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  cursor: pointer;
  border: 2px solid transparent;
  transition: all 0.3s ease;
}

.color-dot:hover {
  border-color: #333;
  transform: scale(1.1);
}

.price {
  font-weight: bold;
  font-size: 24px;
  background: linear-gradient(45deg, #ff6b6b, #ffd93d);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin: 10px 0;
}

.rating {
  color: #ffd93d;
  font-size: 14px;
  margin: 8px 0;
}

.add-to-cart-btn {
  background: linear-gradient(45deg, #667eea, #764ba2);
  color: white;
  padding: 12px 25px;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
  width: 100%;
  margin-top: 15px;
  transition: all 0.3s ease;
}

.add-to-cart-btn:hover {
  transform: scale(1.02);
  box-shadow: 0 5px 20px rgba(102,126,234,0.4);
}

footer {
  background: linear-gradient(90deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
  color: white;
  text-align: center;
  padding: 30px 20px;
  margin-top: 50px;
}

footer h3 {
  margin-bottom: 15px;
}

.footer-links {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 15px 0;
  flex-wrap: wrap;
}

.footer-links a {
  color: #4facfe;
  text-decoration: none;
  transition: all 0.3s ease;
}

.footer-links a:hover {
  color: #ffd93d;
  text-decoration: underline;
}

.payment-methods {
  margin: 15px 0;
}

.payment-icon {
  display: inline-block;
  margin: 0 8px;
  font-size: 24px;
}

.modal {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.7);
  backdrop-filter: blur(5px);
}

.modal.active {
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal-content {
  background: linear-gradient(135deg, #ffffff 0%, #f5f7fa 100%);
  padding: 30px;
  border-radius: 20px;
  width: 90%;
  max-width: 500px;
  max-height: 70vh;
  overflow-y: auto;
  box-shadow: 0 20px 60px rgba(0,0,0,0.3);
}

.modal-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  border-bottom: 3px solid #667eea;
  padding-bottom: 15px;
}

.modal-header h2 {
  color: #1a1a2e;
}

.close-btn {
  font-size: 28px;
  font-weight: bold;
  cursor: pointer;
  background: none;
  border: none;
  color: #666;
  transition: all 0.3s ease;
}

.close-btn:hover {
  color: #ff6b6b;
  transform: scale(1.2);
}

.cart-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 0;
  border-bottom: 1px solid #eee;
}

.cart-item-info {
  text-align: left;
}

.cart-item-name {
  font-weight: bold;
  color: #1a1a2e;
}

.cart-item-price {
  color: #667eea;
  font-size: 14px;
  font-weight: bold;
}

.remove-btn {
  background: #ff6b6b;
  color: white;
  padding: 6px 12px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 12px;
  transition: all 0.3s ease;
}

.remove-btn:hover {
  background: #ff5252;
  transform: scale(1.05);
}

.cart-empty {
  text-align: center;
  padding: 40px 20px;
  color: #666;
}

.cart-total {
  margin-top: 20px;
  padding-top: 20px;
  border-top: 3px solid #667eea;
  font-size: 20px;
  font-weight: bold;
  color: #1a1a2e;
  text-align: right;
}

.checkout-btn {
  width: 100%;
  margin-top: 15px;
  padding: 14px;
  background: linear-gradient(45deg, #ff6b6b, #ff8e72);
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
}

.checkout-btn:hover {
  transform: scale(1.02);
  box-shadow: 0 8px 25px rgba(255,107,107,0.3);
}

.payment-option {
  margin: 10px 0;
  padding: 10px;
  border: 2px solid #ddd;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.payment-option:hover {
  border-color: #667eea;
  background: rgba(102,126,234,0.1);
}

.payment-option input {
  margin-right: 10px;
}

.track-modal-content {
  background: white;
  padding: 30px;
  border-radius: 15px;
  max-width: 600px;
  width: 90%;
}

.order-status {
  margin: 20px 0;
  padding: 15px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border-radius: 10px;
  text-align: center;
}

.status-step {
  display: flex;
  align-items: center;
  margin: 15px 0;
  padding: 10px;
  border-left: 4px solid #667eea;
  background: #f5f7fa;
  border-radius: 5px;
}

.status-step.completed {
  border-left-color: #4caf50;
}

.status-icon {
  font-size: 24px;
  margin-right: 15px;
}

.no-orders {
  text-align: center;
  padding: 40px 20px;
  color: #666;
}

@media (max-width: 768px) {
  .header-left {
    flex-direction: column;
    gap: 10px;
  }

  .search-box {
    max-width: 100%;
  }

  .header-right {
    flex-direction: column;
    width: 100%;
  }

  .hero h1 {
    font-size: 32px;
  }

  .hero-features {
    flex-direction: column;
    gap: 10px;
  }

  .products {
    grid-template-columns: 1fr;
    padding: 20px;
  }
}
</style>
</head>

<body>

<header>
  <div class="header-left">
    <div class="logo">⚡ Las.kys</div>
    <div class="search-box">
      <input type="text" id="searchInput" placeholder="Rechercher un T-shirt..." onkeyup="filterProducts()">
      <button onclick="filterProducts()">🔍</button>
    </div>
  </div>
  <div class="header-right">
    <button class="track-order-btn" onclick="openTrackOrder()">📦 Suivi</button>
    <button class="cart-icon" onclick="openCart()">🛒 Panier (<span id="cart-count">0</span>)</button>
  </div>
</header>

<section class="hero">
  <h1>T-shirts Personnalisés Las.kys</h1>
  <p>Style unique. Qualité premium. Livraison rapide.</p>
  <div class="hero-features">
    <div class="feature">✨ Design Premium</div>
    <div class="feature">🚚 Livraison 48h</div>
    <div class="feature">💯 Qualité Garantie</div>
    <div class="feature">♻️ Éco-Responsable</div>
  </div>
</section>

<section class="products" id="productsContainer">
</section>

<div id="cartModal" class="modal">
  <div class="modal-content">
    <div class="modal-header">
      <h2>Mon Panier 🛒</h2>
      <button class="close-btn" onclick="closeCart()">✕</button>
    </div>
    <div id="cartItems"></div>
    <div class="cart-total">
      Total: <span id="totalPrice">0,00€</span>
    </div>
    
    <h3 style="margin-top: 25px; color: #1a1a2e;">Méthode de paiement</h3>
    <div class="payment-option">
      <input type="radio" name="payment" value="stripe" checked> 💳 Carte Bancaire (Stripe)
    </div>
    <div class="payment-option">
      <input type="radio" name="payment" value="paypal"> 🅿️ PayPal
    </div>
    <div class="payment-option">
      <input type="radio" name="payment" value="virement"> 🏦 Virement Bancaire
    </div>
    
    <button class="checkout-btn" onclick="checkout()">Passer la commande</button>
  </div>
</div>

<div id="trackModal" class="modal">
  <div class="track-modal-content">
    <div class="modal-header">
      <h2>Suivi de Commande 📦</h2>
      <button class="close-btn" onclick="closeTrackOrder()">✕</button>
    </div>
    <div id="trackContent"></div>
  </div>
</div>

<footer>
  <h3>Las.kys - Boutique de T-shirts Premium</h3>
  
  <div class="payment-methods">
    <strong>Paiements acceptés :</strong><br>
    <span class="payment-icon">💳</span>
    <span class="payment-icon">🅿️</span>
    <span class="payment-icon">🏦</span>
  </div>
  
  <div class="footer-links">
    <a href="#about">À propos</a>
    <a href="#contact">Contact</a>
    <a href="#privacy">Confidentialité</a>
    <a href="#terms">Conditions</a>
    <a href="#shipping">Livraison</a>
    <a href="#returns">Retours</a>
  </div>
  
  <p>📞 Contact : kylianengoki@gmail.com</p>
  <p>© 2026 Las.kys - Tous droits réservés ✨</p>
</footer>

<script>
const products = [
  { id: 1, name: 'T-shirt Noir Minimal', price: 29.99, color: 'Noir', rating: '★★★★★', tag: 'Best Seller', colors: ['#000', '#333'], image: 'https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?w=500&h=500&fit=crop' },
  { id: 2, name: 'T-shirt Blanc Street', price: 34.99, color: 'Blanc', rating: '★★★★★', tag: 'Nouveau', colors: ['#FFF', '#f0f0f0'], image: 'https://images.unsplash.com/photo-1503341455253-b2e723bb12dd?w=500&h=500&fit=crop' },
  { id: 3, name: 'T-shirt Beige Luxe', price: 39.99, color: 'Beige', rating: '★★★★☆', tag: 'Premium', colors: ['#D4A574', '#C2A47A'], image: 'https://images.unsplash.com/photo-1618354691551-d1a50ddf06d9?w=500&h=500&fit=crop' },
  { id: 4, name: 'T-shirt Bleu Ocean', price: 32.99, color: 'Bleu', rating: '★★★★★', tag: 'Populaire', colors: ['#1E3A8A', '#2563EB'], image: 'https://images.unsplash.com/photo-1550508739-b0a4603778a5?w=500&h=500&fit=crop' },
  { id: 5, name: 'T-shirt Rouge Passion', price: 34.99, color: 'Rouge', rating: '★★★★☆', tag: 'Tendance', colors: ['#DC2626', '#EF4444'], image: 'https://images.unsplash.com/photo-1597909415171-4aca2e6906dc?w=500&h=500&fit=crop' },
  { id: 6, name: 'T-shirt Vert Naturel', price: 33.99, color: 'Vert', rating: '★★★★★', tag: 'Éco', colors: ['#15803D', '#22C55E'], image: 'https://images.unsplash.com/photo-1514320291840-2e0a9bf2a9ae?w=500&h=500&fit=crop' },
  { id: 7, name: 'T-shirt Gris Intemporel', price: 28.99, color: 'Gris', rating: '★★★★☆', tag: 'Classique', colors: ['#4B5563', '#6B7280'], image: 'https://images.unsplash.com/photo-1552374196-c4029a5f1f3d?w=500&h=500&fit=crop' },
  { id: 8, name: 'T-shirt Purple Mystère', price: 36.99, color: 'Violet', rating: '★★★★★', tag: 'Exclusif', colors: ['#6B21A8', '#A855F7'], image: 'https://images.unsplash.com/photo-1618359266876-461f3291ebc5?w=500&h=500&fit=crop' },
  { id: 9, name: 'T-shirt Rose Candy', price: 31.99, color: 'Rose', rating: '★★★★☆', tag: 'Nouveau', colors: ['#BE185D', '#EC4899'], image: 'https://images.unsplash.com/photo-1494322199015-e3a95b33a237?w=500&h=500&fit=crop' },
  { id: 10, name: 'T-shirt Orange Soleil', price: 33.99, color: 'Orange', rating: '★★★★★', tag: 'Tendance', colors: ['#B45309', '#F97316'], image: 'https://images.unsplash.com/photo-1548126328-c9fa89d128fa?w=500&h=500&fit=crop' },
  { id: 11, name: 'T-shirt Cyan Futuriste', price: 37.99, color: 'Cyan', rating: '★★★★★', tag: 'Premium', colors: ['#0891B2', '#06B6D4'], image: 'https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?w=500&h=500&fit=crop' },
  { id: 12, name: 'T-shirt Marron Vintage', price: 35.99, color: 'Marron', rating: '★★★☆☆', tag: 'Vintage', colors: ['#78350F', '#92400E'], image: 'https://images.unsplash.com/photo-1542119018-02ea4a78d1c7?w=500&h=500&fit=crop' },
];

let cart = [];
let orders = [];

function generateProducts() {
  const container = document.getElementById('productsContainer');
  container.innerHTML = products.map(product => `
    <div class="product">
      <img src="${product.image}" alt="${product.name}" class="product-image" onerror="this.src='https://via.placeholder.com/500x500?text=${encodeURIComponent(product.name)}'">
      <span class="product-tag">${product.tag}</span>
      <h2>${product.name}</h2>
      <div class="product-color">Couleur: ${product.color}</div>
      <div class="colors">
        ${product.colors.map((col, idx) => `<div class="color-dot" style="background: ${col}; border-color: #333;" title="Couleur ${idx + 1}"></div>`).join('')}
      </div>
      <div class="price">${product.price.toFixed(2)}€</div>
      <div class="rating">${product.rating}</div>
      <button class="add-to-cart-btn" onclick="addToCart('${product.name}', ${product.price})">Ajouter au panier</button>
    </div>
  `).join('');
}

function filterProducts() {
  const searchTerm = document.getElementById('searchInput').value.toLowerCase();
  const filtered = products.filter(p => 
    p.name.toLowerCase().includes(searchTerm) || 
    p.color.toLowerCase().includes(searchTerm)
  );
  
  const container = document.getElementById('productsContainer');
  if (filtered.length === 0) {
    container.innerHTML = '<div style="grid-column: 1/-1; text-align: center; padding: 40px; color: white; font-size: 18px;">Aucun produit trouvé 😢</div>';
  } else {
    container.innerHTML = filtered.map(product => `
      <div class="product">
        <img src="${product.image}" alt="${product.name}" class="product-image" onerror="this.src='https://via.placeholder.com/500x500?text=${encodeURIComponent(product.name)}'">
        <span class="product-tag">${product.tag}</span>
        <h2>${product.name}</h2>
        <div class="product-color">Couleur: ${product.color}</div>
        <div class="colors">
          ${product.colors.map((col, idx) => `<div class="color-dot" style="background: ${col}; border-color: #333;" title="Couleur ${idx + 1}"></div>`).join('')}
        </div>
        <div class="price">${product.price.toFixed(2)}€</div>
        <div class="rating">${product.rating}</div>
        <button class="add-to-cart-btn" onclick="addToCart('${product.name}', ${product.price})">Ajouter au panier</button>
      </div>
    `).join('');
  }
}

function addToCart(name, price) {
  cart.push({ name, price, id: Date.now() });
  document.getElementById('cart-count').textContent = cart.length;
  updateCartDisplay();
  showNotification(`${name} ajouté au panier ! ✓`);
}

function removeFromCart(id) {
  cart = cart.filter(item => item.id !== id);
  document.getElementById('cart-count').textContent = cart.length;
  updateCartDisplay();
}

function updateCartDisplay() {
  const cartItemsDiv = document.getElementById('cartItems');
  
  if (cart.length === 0) {
    cartItemsDiv.innerHTML = '<div class="cart-empty">Votre panier est vide 😢<br>Découvrez nos superbes T-shirts !</div>';
    document.getElementById('totalPrice').textContent = '0,00€';
    return;
  }
  
  let html = '';
  let total = 0;
  
  cart.forEach(item => {
    html += `
      <div class="cart-item">
        <div class="cart-item-info">
          <div class="cart-item-name">${item.name}</div>
          <div class="cart-item-price">${item.price.toFixed(2)}€</div>
        </div>
        <button class="remove-btn" onclick="removeFromCart(${item.id})">✕ Supprimer</button>
      </div>
    `;
    total += item.price;
  });
  
  cartItemsDiv.innerHTML = html;
  document.getElementById('totalPrice').textContent = total.toFixed(2) + '€';
}

function openCart() {
  document.getElementById('cartModal').classList.add('active');
}

function closeCart() {
  document.getElementById('cartModal').classList.remove('active');
}

function checkout() {
  if (cart.length === 0) {
    alert('Votre panier est vide !');
    return;
  }
  
  const paymentMethod = document.querySelector('input[name="payment"]:checked').value;
  const total = cart.reduce((sum, item) => sum + item.price, 0);
  const orderId = 'LK-' + Math.random().toString(36).substr(2, 9).toUpperCase();
  
  let paymentText = '';
  if (paymentMethod === 'stripe') {
    paymentText = '💳 Redirection vers Stripe sécurisé...';
  } else if (paymentMethod === 'paypal') {
    paymentText = '🅿️ Redirection vers PayPal...';
  } else {
    paymentText = '🏦 Détails du virement envoyés par email';
  }
  
  const order = {
    id: orderId,
    items: [...cart],
    total: total,
    date: new Date().toLocaleDateString('fr-FR'),
    status: 'Confirmée',
    paymentMethod: paymentMethod
  };
  
  orders.push(order);
  localStorage.setItem('orders', JSON.stringify(orders));
  
  alert(`✅ Commande confirmée !\n\nN° Commande: ${orderId}\nTotal: ${total.toFixed(2)}€\n\n${paymentText}\n\nVous recevrez un email de confirmation avec le lien de suivi.`);
  
  cart = [];
  document.getElementById('cart-count').textContent = '0';
  updateCartDisplay();
  closeCart();
}

function openTrackOrder() {
  const trackContent = document.getElementById('trackContent');
  const savedOrders = JSON.parse(localStorage.getItem('orders') || '[]');
  
  if (savedOrders.length === 0) {
    trackContent.innerHTML = '<div class="no-orders">📦 Aucune commande trouvée.<br><br>Passez votre première commande dès maintenant !</div>';
  } else {
    let html = '';
    savedOrders.forEach(order => {
      const itemsList = order.items.map(item => `• ${item.name} (${item.price.toFixed(2)}€)`).join('<br>');
      html += `
        <div class="order-status">
          <strong>Commande ${order.id}</strong><br>
          📅 ${order.date} | 💰 ${order.total.toFixed(2)}€
        </div>
        <div style="margin: 15px 0; font-size: 14px; color: #666;">
          <strong>Articles:</strong><br>${itemsList}
        </div>
        <div class="status-step completed">
          <span class="status-icon">✅</span>
          <strong>Commande Confirmée</strong><br>
          <small>Paiement reçu</small>
        </div>
        <div class="status-step completed">
          <span class="status-icon">📦</span>
          <strong>En Préparation</strong><br>
          <small>Emballage en cours</small>
        </div>
        <div class="status-step">
          <span class="status-icon">🚚</span>
          <strong>En Livraison</strong><br>
          <small>Sera expédié dans 48h</small>
        </div>
        <div class="status-step">
          <span class="status-icon">🏠</span>
          <strong>Livré</strong><br>
          <small>À votre porte</small>
        </div>
        <hr style="margin: 20px 0;">
      `;
    });
    trackContent.innerHTML = html;
  }
  
  document.getElementById('trackModal').classList.add('active');
}

function closeTrackOrder() {
  document.getElementById('trackModal').classList.remove('active');
}

function showNotification(message) {
  const notif = document.createElement('div');
  notif.style.cssText = 'position: fixed; top: 80px; right: 20px; background: #4caf50; color: white; padding: 15px 25px; border-radius: 8px; z-index: 2000;';
  notif.textContent = message;
  document.body.appendChild(notif);
  setTimeout(() => notif.remove(), 3000);
}

window.onclick = function(event) {
  const cartModal = document.getElementById('cartModal');
  const trackModal = document.getElementById('trackModal');
  if (event.target === cartModal) cartModal.classList.remove('active');
  if (event.target === trackModal) trackModal.classList.remove('active');
}

orders = JSON.parse(localStorage.getItem('orders') || '[]');
generateProducts();
</script>

</body>
</html>
