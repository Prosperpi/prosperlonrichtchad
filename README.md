Doc
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dentifrice Thé Blanc Multi-Effet - Longrich Tchad</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Longrich Tchad</h1>
  </header>

  <main>
    <article>
      <h1>Dentifrice White Tea Multi-Effect</h1>

      <!-- BOITE 1 : PHOTO -->
      <section id="photo-produit">
        <h2>Image produit</h2>
        <img src="longrich-white-tea.jpg" alt="Boîte de Dentifrice Longrich White Tea Multi-Effect 120g">
      </section>

      <!-- BOITE 2 : PRIX -->
      <section id="prix">
        <h2>Prix</h2>
        <p><strong>5 000 FCFA</strong></p>
        <p><small>TVA incluse. Livraison à N'Djamena : 500 FCFA</small></p>
      </section>

      <!-- BOITE 3 : ACTION -->
      <section id="action">
        <h2>Commander</h2>
        <button type="button" id="btnPanier">Ajouter au panier</button>
        <button type="button" id="btnAcheter">Acheter maintenant</button>
        <p id="message"></p>
      </section>

      <!-- BOITE 4 : DESCRIPTION -->
      <section id="description">
        <h2>Atouts clés</h2>
        <ul>
          <li>Formule Multi-Effet : Blanchit et protège</li>
          <li>Extrait de Thé Blanc</li>
          <li>Sans SLS. Haleine fraîche</li>
        </ul>
      </section>
    </article>
  </main>

  <footer>
    <p>&copy; 2026 Longrich Tchad - Réalisé par YANYAHKA KEUMO PROSPER</p>
  </footer>
  <script src="script.js"></script>
</body>
</html>
:root{--vert:#0a7a0a; --gris:#f5f5f5}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:system-ui,Arial,sans-serif;background:var(--gris);color:#222;line-height:1.5}
header{background:var(--vert);color:white;text-align:center;padding:1rem}
main{max-width:600px;margin:1rem auto;padding:1rem;background:white;border-radius:8px}
h1{font-size:1.4rem;margin-bottom:0.5rem}
h2{font-size:1.1rem;color:var(--vert);margin-top:1rem}
img{max-width:100%;height:auto;border-radius:6px}
section{margin-bottom:1.5rem}
button{background:var(--vert);color:white;border:none;padding:12px 18px;border-radius:6px;cursor:pointer;margin-right:0.5rem;font-weight:600}
button:hover{opacity:0.9}
footer{text-align:center;padding:1rem;font-size:0.9rem;color:#555}

const msg = document.getElementById("message");

document.getElementById("btnPanier").addEventListener("click", () => {
  msg.innerText = "Produit ajouté au panier ✓";
  msg.style.color = "green";
});

document.getElementById("btnAcheter").addEventListener("click", () => {
  msg.innerText = "Redirection vers WhatsApp pour commander...";
  msg.style.color = "green";
});
