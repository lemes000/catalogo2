<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doces Gourmet da Su</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Doces Gourmet da Su</h1>
        <p>Delícias que derretem na boca!</p>
    </header>
    
    <main>
        <section class="products">
            <h2>Nossos Produtos</h2>
            <div class="product">
                <h3>Cone Recheado</h3>
                <p>Sabores: Brigadeiro, Ninho com Nutella, Doce de Leite, Ferrero Rocher, Rafaello, Beijinho</p>
                <button onclick="addToCart('Cone Recheado')">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <h3>Trufas</h3>
                <p>Sabores: Brigadeiro, Ninho com Nutella, Doce de Leite, Ferrero Rocher, Rafaello, Beijinho</p>
                <button onclick="addToCart('Trufas')">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <h3>Bombom de Oreo</h3>
                <p>Uma explosão de sabor em cada mordida!</p>
                <button onclick="addToCart('Bombom de Oreo')">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <h3>Coxinha de Morango</h3>
                <p>Uma combinação deliciosa de doce e crocante!</p>
                <button onclick="addToCart('Coxinha de Morango')">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <h3>Cestinha de Morango com Creme de Ninho e Nutella</h3>
                <p>Um doce irresistível que vai conquistar seu paladar!</p>
                <button onclick="addToCart('Cestinha de Morango')">Adicionar ao Carrinho</button>
            </div>
            <div class="product">
                <h3>Bombom de Uva no Pote</h3>
                <p>Uma sobremesa prática e deliciosa para compartilhar!</p>
                <button onclick="addToCart('Bombom de Uva')">Adicionar ao Carrinho</button>
            </div>
        </section>

        <section class="checkout">
            <h2>Finalizar Compra</h2>
            <p>Para finalizar sua compra, clique no botão abaixo:</p>
            <button onclick="finalizarCompra()">Finalizar Compra</button>
        </section>

        <section class="share">
            <h2>Compartilhe o Site</h2>
            <button onclick="shareWhatsApp()">Compartilhar no WhatsApp</button>
            <button onclick="copyLink()">Copiar Link</button>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Doces Gourmet da Su - Todos os direitos reservados.</p>
    </footer>

    <script>
        let cart = [];

        function addToCart(product) {
            cart.push(product);
            alert(product + " adicionado ao carrinho!");
        }

        function finalizarCompra() {
            if (cart.length === 0) {
                alert("Seu carrinho está vazio!");
                return;
            }
            const mensagem = "Olá, gostaria de fazer um pedido: " + cart.join(", ");
            const whatsappUrl = `https://wa.me/5518997830438?text=${encodeURIComponent(mensagem)}`;
            window.open(whatsappUrl, '_blank');
        }

        function shareWhatsApp() {
            const url = window.location.href; // Pega o link atual do site
            const mensagem = "Confira este site incrível de doces: " + url;
            const whatsappUrl = `https://wa.me/?text=${encodeURIComponent(mensagem)}`;
            window.open(whatsappUrl, '_blank');
        }

        function copyLink() {
            const url = window.location.href; // Pega o link atual do site
            navigator.clipboard.writeText(url).then(() => {
                alert("Link copiado para a área de transferência!");
            }).catch(err => {
                alert("Erro ao copiar o link.");
            });
        }
    </script>
</body>
</html>
