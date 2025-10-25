# Clone
Clone cc
<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Checkout — Mock</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="page">
    <div class="checkout-card" role="region" aria-label="Mock do Checkout">
      <header class="card-header">
        <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='120' height='28'><rect width='120' height='28' fill='%23222'/><text x='12' y='18' fill='%23fff' font-family='Arial' font-size='14'>Loja - Checkout</text></svg>" alt="Logo" class="logo">
        <div class="secure">Pagamento seguro</div>
      </header>

      <main class="card-body">
        <section class="item">
          <img class="thumb" src="https://images.unsplash.com/photo-1582582494706-9bb9b1b8b6a9?w=800&q=60&auto=format&fit=crop" alt="Produto">
          <div class="meta">
            <div class="title">Sofá Moderno — 3 lugares</div>
            <div class="subtitle">Quantidade: 1</div>
          </div>
          <div class="price">R$ 1.299,00</div>
        </section>

        <section class="summary">
          <div><span>Subtotal</span><span>R$ 1.299,00</span></div>
          <div><span>Frete</span><span>R$ 0,00</span></div>
          <div class="total"><span>Total</span><span>R$ 1.299,00</span></div>
        </section>

        <section class="payment">
          <h4>Método de pagamento</h4>
          <div class="payment-box">
            <label class="pm mock">
              <input type="radio" name="pm" checked disabled>
              <span>Cartão de crédito •••• 4242</span>
            </label>
            <button id="simulateBtn" class="pay-btn">Simular pagamento</button>
            <p class="note">Este é um mock visual. Não insira dados reais.</p>
          </div>
        </section>
      </main>

      <footer class="card-footer">
        <small>Suporte • Política de reembolso • Termos</small>
      </footer>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
