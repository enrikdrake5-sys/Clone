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
</html>:root{--bg:#f6f7f9;--card:#fff;--accent:#635bff;--muted:#6b7280}
*{box-sizing:border-box}
body,html{height:100%;margin:0;font-family:Inter,system-ui,Arial,Helvetica,sans-serif;background:var(--bg);color:#111}
.page{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:24px}
.checkout-card{width:420px;background:var(--card);border-radius:12px;box-shadow:0 10px 30px rgba(15,23,42,0.08);overflow:hidden;display:flex;flex-direction:column}
.card-header{display:flex;align-items:center;justify-content:space-between;padding:18px 20px;border-bottom:1px solid #eef0f3}
.logo{height:28px}
.secure{font-size:13px;color:var(--muted)}
.card-body{padding:18px 20px;display:flex;flex-direction:column;gap:14px}
.item{display:flex;gap:12px;align-items:center}
.thumb{width:64px;height:64px;border-radius:8px;object-fit:cover}
.meta{flex:1}
.title{font-weight:600}
.subtitle{font-size:13px;color:var(--muted);margin-top:6px}
.price{font-weight:700;color:var(--accent)}
.summary{background:#fbfcff;padding:12px;border-radius:8px;border:1px solid #f0f2fb}
.summary div{display:flex;justify-content:space-between;margin:6px 0}
.total{font-weight:800}
.payment h4{margin:0 0 8px 0}
.payment-box{display:flex;flex-direction:column;gap:10px}
.pm{display:flex;align-items:center;gap:10px;background:#fff;padding:10px;border-radius:8px;border:1px solid #eceef6}
.pay-btn{background:var(--accent);color:#fff;border:0;padding:12px;border-radius:8px;font-weight:700;cursor:pointer}
.note{font-size:12px;color:var(--muted)}
.card-footer{padding:12px 20px;border-top:1px solid #eef0f3;text-align:center;font-size:13px;color:var(--muted)}
@media (max-width:480px){.checkout-card{width:100%}}document.getElementById('simulateBtn').addEventListener('click', function(){
  alert('Pagamento simulado com sucesso. (Mock apenas — sem transações reais.)');
});


