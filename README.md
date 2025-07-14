<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kakau Pizzas - Cucina artigianale e pizzeria | Poxoréu - mt</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
	
  <meta property="og:title" content="Kakau Pizzas - Cucina artigianale e pizzeria. Kakau Pizzas - Pizzaria Artesanal. Especialista em pizzas caseiras doces e salgadas">

  <meta property="og:description" content="Pizzas Artesanal de sabor irresistível, produzidas com muito amor e atenção aos detalhes e inspirados no estino italiano!">
  <meta property="og:image" content="">
  <meta property="og:url" content="https://instagram.com/kakau_pizzas">
  <meta property="og:type" content="website">
  <link rel="canonical" href="https://www.exemplo.com/url-oficial/" />

    
    <style>
        :root {
            --color-primary: #a72a2a; /* Vermelho Italiano */
            --color-secondary: #4a913c; /* Verde Italiano */
            --color-light: #f8f8f8; /* Branco Suave */
            --color-dark: #333;
            --color-gray: #eee;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.6;
            color: var(--color-dark);
            background-color: var(--color-light);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: auto;
            overflow: hidden;
        }

        /* Header */
        header {
            background-color: var(--color-light);
            padding: 1rem 0;
            border-bottom: 2px solid var(--color-gray);
            text-align: center;
        }

        header h2 {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5rem;
            color: var(--color-primary);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }

        /* Navbar */
        nav {
            background-color: var(--color-secondary);
            color: var(--color-light);
            padding: 0.8rem 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 999;
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: var(--color-light);
            text-decoration: none;
            font-weight: bold;
            padding: 5px 0;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        nav ul li a:hover {
            color: var(--color-primary);
            transform: translateY(-2px);
        }

        /* Mobile Menu Button */
        .menu-toggle {
            display: none;
            flex-direction: column;
            cursor: pointer;
            padding: 10px;
            position: absolute;
            top: 25px;
            right: 20px;
            z-index: 1000;
        }

        .menu-toggle span {
            height: 3px;
            width: 25px;
            background: var(--color-primary);
            margin-bottom: 4px;
            border-radius: 5px;
            transition: all 0.3s ease;
        }

        /* Sections */
        section {
            padding: 40px 0;
            text-align: center;
        }

        section:nth-of-type(even) {
            background-color: var(--color-gray);
        }

        h1, h3 {
            color: var(--color-primary);
            margin-bottom: 20px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
        }

        p {
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .highlight-text {
            font-weight: bold;
            font-style: italic;
        }

        /* Modal */
        .modal {
            display: none;
            position: fixed;
            z-index: 1001;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.6);
            display: flex; /* Para centralizar o conteúdo */
            align-items: center;
            justify-content: center;
        }

        .modal-content {
            background-color: var(--color-light);
            margin: 15% auto; /* Ajustado para centralização flex */
            padding: 30px;
            border: 1px solid var(--color-secondary);
            width: 80%;
            max-width: 500px;
            text-align: center;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            position: relative;
            animation: fadeIn 0.5s;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .modal-content h3 {
            color: var(--color-secondary);
            margin-bottom: 20px;
        }

        .modal-content p {
            font-size: 1.2rem;
            color: var(--color-dark);
        }

        /* Nossas Pizzas Section */
        .pizza-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .pizza-item {
            background-color: var(--color-light);
            border: 1px solid var(--color-gray);
            border-radius: 8px;
            padding: 20px;
            text-align: left;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .pizza-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.15);
        }

        .pizza-item h4 {
            color: var(--color-primary);
            margin-bottom: 10px;
            font-size: 1.4rem;
        }

        .pizza-item p {
            font-size: 0.95rem;
            color: #555;
            margin-bottom: 5px;
        }

        .pizza-item .price {
            font-weight: bold;
            color: var(--color-secondary);
            margin-top: 10px;
            font-size: 1.1rem;
        }

        .pizza-item .brotinho-price {
            font-size: 0.9rem;
            color: #777;
            margin-top: 5px;
        }

        /* Pedidos Section */
        #pedidos form {
            background-color: var(--color-light);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            max-width: 700px;
            margin: 30px auto;
            text-align: left;
        }

        #pedidos label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: var(--color-dark);
        }

        #pedidos select,
        #pedidos input[type="number"],
        #pedidos input[type="text"] {
            width: calc(100% - 20px);
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid var(--color-secondary);
            border-radius: 8px;
            font-size: 1rem;
            background-color: var(--color-light);
        }

        #pedidos input[type="checkbox"] {
            margin-right: 10px;
        }

        #pedidos .form-group {
            margin-bottom: 20px;
        }

        #pedidos .radio-group label {
            display: inline-block;
            margin-right: 20px;
        }

        #pedidos .pizza-selection-group,
        #pedidos .borda-selection-group {
            border: 1px solid var(--color-gray);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 25px;
            background-color: #fcfcfc;
        }

        #pedidos .pizza-selection-group h4,
        #pedidos .borda-selection-group h4 {
            color: var(--color-secondary);
            margin-top: 0;
            margin-bottom: 15px;
            font-size: 1.2rem;
        }

        #pedidos .item-selection {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
            flex-wrap: wrap;
        }

        #pedidos .item-selection label {
            margin-bottom: 0;
            flex: 1;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        #pedidos .item-selection input[type="number"] {
            width: 70px;
            margin-left: 10px;
            margin-bottom: 0;
            text-align: center;
        }

        #pedidos button {
            background-color: var(--color-primary);
            color: var(--color-light);
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            width: 100%;
        }

        #pedidos button:hover {
            background-color: #8c2121;
            transform: translateY(-2px);
        }

        #orderSummary {
            background-color: var(--color-light);
            padding: 20px;
            border-radius: 10px;
            border: 1px dashed var(--color-secondary);
            margin-top: 30px;
            font-size: 1.1rem;
            color: var(--color-dark);
            text-align: left;
            display: none; /* Hidden by default */
        }

        #orderSummary h4 {
            color: var(--color-secondary);
            margin-bottom: 10px;
        }

        /* Contact Section */
        #contato .contact-info {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        #contato .contact-item {
            text-align: center;
            padding: 20px;
            background-color: var(--color-light);
            border: 1px solid var(--color-gray);
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            width: 250px;
            transition: transform 0.3s ease;
        }

        #contato .contact-item:hover {
            transform: translateY(-5px);
        }

        #contato .contact-item i {
            font-size: 2.5rem;
            color: var(--color-primary);
            margin-bottom: 15px;
        }

        #contato .contact-item a {
            color: var(--color-dark);
            text-decoration: none;
            font-weight: bold;
        }

        #contato .contact-item a:hover {
            color: var(--color-secondary);
        }

        #contato form {
            background-color: var(--color-light);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            max-width: 600px;
            margin: 40px auto;
            text-align: left;
        }

        #contato form label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: var(--color-dark);
        }

        #contato form input[type="text"],
        #contato form input[type="email"],
        #contato form textarea {
            width: calc(100% - 20px);
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid var(--color-secondary);
            border-radius: 8px;
            font-size: 1rem;
            background-color: var(--color-light);
        }

        #contato form textarea {
            resize: vertical;
            min-height: 100px;
        }

        #contato form button {
            background-color: var(--color-primary);
            color: var(--color-light);
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            width: 100%;
        }

        #contato form button:hover {
            background-color: #8c2121;
            transform: translateY(-2px);
        }

        /* Footer */
        footer {
            background-color: var(--color-dark);
            color: var(--color-light);
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }

        footer p {
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        footer a {
            color: var(--color-secondary);
            text-decoration: none;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: var(--color-primary);
        }

        /* Responsiveness */
        @media (max-width: 768px) {
            header h2 {
                font-size: 2.5rem;
            }

            nav ul {
                flex-direction: column;
                display: none; /* Hide by default for mobile */
                width: 100%;
                background-color: var(--color-secondary);
                position: absolute;
                top: 75px; /* Adjust based on header height */
                left: 0;
                z-index: 999;
            }

            nav ul.active {
                display: flex;
            }

            nav ul li {
                margin: 10px 0;
            }

            .menu-toggle {
                display: flex;
            }

            .menu-toggle.active span:nth-child(1) {
                transform: rotate(45deg) translate(5px, 5px);
            }
            .menu-toggle.active span:nth-child(2) {
                opacity: 0;
            }
            .menu-toggle.active span:nth-child(3) {
                transform: rotate(-45deg) translate(5px, -5px);
            }

            .modal-content {
                width: 90%;
                margin: 10% auto;
            }

            .pizza-grid {
                grid-template-columns: 1fr;
            }

            #pedidos .item-selection {
                flex-direction: column;
                align-items: flex-start;
            }

            #pedidos .item-selection input[type="number"] {
                width: 100%;
                margin-left: 0;
                margin-top: 5px;
            }

            #pedidos .item-selection label[for^="brotinho"] {
                margin-left: 0;
                margin-top: 5px;
            }
        }
    </style>
</head>
<body>

    <div id="welcomeModal" class="modal">
        <div class="modal-content">
            <h3>Bem-vindo(a) à Kakau Pizzas!</h3>
            <p><span class="highlight-text">Mês de inauguração da Kakau Pizzas: Cucina artigianale e pizzeria.</span> Na compra de três pizzas, ganhe um brotinho doce no sabor que você desejar!</p>
            <p>Clique em qualquer lugar para continuar.</p>
        </div>
    </div>

    <header>
        <div class="container">
            <h2>Kakau Pizzas - Cucina artigianale e pizzeria</h2>
        </div>
    </header>

    <nav>
        <div class="container">
            <div class="menu-toggle" id="mobile-menu">
                <span></span>
                <span></span>
                <span></span>
            </div>
            <ul id="navbar-links">
                <li><a href="#inicial">Inicial</a></li>
                <li><a href="#sobre-nos">Sobre nós</a></li>
                <li><a href="#nossas-pizzas">Nossas Pizzas</a></li>
                <li><a href="#pedidos">Pedidos</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </div>
    </nav>

    <main>
        <section id="inicial">
            <div class="container">
                <h1>Bem-vindo à Kakau Pizzas!</h1>
                <p>Descubra os sabores irresistíveis de nossas pizzas artesanais!</p>
            </div>
        </section>

        <hr>

        <section id="sobre-nos">
            <div class="container">
                <h3>Sobre Nós</h3>
                <p>Na Kakau Pizzas, acreditamos que a melhor pizza é feita com carinho, ingredientes simples e um toque artesanal. Nossa produção é totalmente caseira, valorizando cada detalhe para garantir que você tenha a melhor experiência em sabor. Nossas massas são preparadas com dedicação e os ingredientes selecionados para te proporcionar uma explosão de sabor em cada mordida. Venha experimentar nossas pizzas, feitas com alma e sabor!</p>
                <br>
                <h3>Horário de Funcionamento para Pedidos e Encomendas</h3>
                <p><span class="highlight-text">Horário de funcionamento:</span> 17h00 às 22h00</p>
                <p><span class="highlight-text">Pedidos somente de:</span> Segunda-feira a Quinta-feira</p>
                <p><span class="highlight-text">Entregas:</span> Sexta-feira, Sábado e Domingo</p>
            </div>
        </section>

        <hr>

        <section id="nossas-pizzas">
            <div class="container">
                <h3>Nossas Pizzas</h3>
                <p>Confira a nossa seleção de pizzas doces e salgadas, disponíveis também na versão brotinho!</p>

                <h4>Pizzas Salgadas</h4>
                <div class="pizza-grid">
                    <div class="pizza-item">
                        <h4>1. Mussarela Tradicional</h4>
                        <p>Molho de tomate, mussarela, azeitonas e orégano.</p>
                        <p class="price">Tamanho médio/grande: R$55,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$19,25</p>
                    </div>
                    <div class="pizza-item">
                        <h4>2. Calabresa</h4>
                        <p>Molho de tomate, mussarela, linguiça calabresa fatiada, cebola e orégano.</p>
                        <p class="price">Tamanho médio/grande: R$60,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$21,00</p>
                    </div>
                    <div class="pizza-item">
                        <h4>3. Presunto e Queijo</h4>
                        <p>Molho de tomate, mussarela, presunto fatiado/picado e orégano.</p>
                        <p class="price">Tamanho médio/grande: R$58,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$20,30</p>
                    </div>
                    <div class="pizza-item">
                        <h4>4. Vegetariano de Legumes</h4>
                        <p>Molho de tomate, mussarela, ervilha, cenoura, batata e orégano.</p>
                        <p class="price">Tamanho médio/grande: R$60,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$21,00</p>
                    </div>
                    <div class="pizza-item">
                        <h4>5. Portuguesa (Especial da Kakau)</h4>
                        <p>Molho de tomate, mussarela, presunto, ovos cozidos picados, cebola em rodelas, azeitonas e orégano.</p>
                        <p class="price">Tamanho médio/grande: R$67,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$23,45</p>
                    </div>
                </div>

                <h4 style="margin-top: 40px;">Pizzas Doces</h4>
                <div class="pizza-grid">
                    <div class="pizza-item">
                        <h4>6. Chocolate</h4>
                        <p>Chocolate ao leite e granulado.</p>
                        <p class="price">Tamanho médio/grande: R$45,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$15,75</p>
                    </div>
                    <div class="pizza-item">
                        <h4>7. Doce Pecado</h4>
                        <p>Morango em cortes e chocolate ao leite.</p>
                        <p class="price">Tamanho médio/grande: R$55,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$19,25</p>
                    </div>
                    <div class="pizza-item">
                        <h4>8. Romeu e Julieta</h4>
                        <p>Doce de goiabada e queijo.</p>
                        <p class="price">Tamanho médio/grande: R$43,00</p>
                        <p class="brotinho-price">Versão Brotinho (25cm - 4 fatias): R$15,05</p>
                    </div>
                </div>
            </div>
        </section>

        <hr>

        <section id="pedidos">
            <div class="container">
                <h3>Faça Seu Pedido</h3>
                <form id="orderForm">
                    <div class="form-group">
                        <label>Tipo de Pizza:</label>
                        <div class="radio-group">
                            <input type="radio" id="pizzaTypeSalgada" name="pizzaType" value="salgada" checked>
                            <label for="pizzaTypeSalgada">Somente Salgada</label>
                            <input type="radio" id="pizzaTypeDoce" name="pizzaType" value="doce">
                            <label for="pizzaTypeDoce">Somente Doce</label>
                            <input type="radio" id="pizzaTypeAmbas" name="pizzaType" value="ambas">
                            <label for="pizzaTypeAmbas">Ambas (Salgada e Doce)</label>
                        </div>
                    </div>

                    <div class="pizza-selection-group" id="salgadaPizzas">
                        <h4>Pizzas Salgadas</h4>
                        <div class="item-selection">
                            <label for="qtyMussarela">1. Mussarela Tradicional (R$55,00 / Brotinho R$19,25)</label>
                            <input type="number" id="qtyMussarela" min="0" value="0" data-price="55.00" data-brotinho-price="19.25">
                            <input type="checkbox" id="brotinhoMussarela"> <label for="brotinhoMussarela" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyCalabresa">2. Calabresa (R$60,00 / Brotinho R$21,00)</label>
                            <input type="number" id="qtyCalabresa" min="0" value="0" data-price="60.00" data-brotinho-price="21.00">
                            <input type="checkbox" id="brotinhoCalabresa"> <label for="brotinhoCalabresa" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyPresunto">3. Presunto e Queijo (R$58,00 / Brotinho R$20,30)</label>
                            <input type="number" id="qtyPresunto" min="0" value="0" data-price="58.00" data-brotinho-price="20.30">
                            <input type="checkbox" id="brotinhoPresunto"> <label for="brotinhoPresunto" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyVegetariano">4. Vegetariano de Legumes (R$60,00 / Brotinho R$21,00)</label>
                            <input type="number" id="qtyVegetariano" min="0" value="0" data-price="60.00" data-brotinho-price="21.00">
                            <input type="checkbox" id="brotinhoVegetariano"> <label for="brotinhoVegetariano" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyPortuguesa">5. Portuguesa (R$67,00 / Brotinho R$23,45)</label>
                            <input type="number" id="qtyPortuguesa" min="0" value="0" data-price="67.00" data-brotinho-price="23.45">
                            <input type="checkbox" id="brotinhoPortuguesa"> <label for="brotinhoPortuguesa" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                    </div>

                    <div class="pizza-selection-group" id="docePizzas" style="display: none;">
                        <h4>Pizzas Doces</h4>
                        <div class="item-selection">
                            <label for="qtyChocolate">6. Chocolate (R$45,00 / Brotinho R$15,75)</label>
                            <input type="number" id="qtyChocolate" min="0" value="0" data-price="45.00" data-brotinho-price="15.75">
                            <input type="checkbox" id="brotinhoChocolate"> <label for="brotinhoChocolate" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyDocePecado">7. Doce Pecado (R$55,00 / Brotinho R$19,25)</label>
                            <input type="number" id="qtyDocePecado" min="0" value="0" data-price="55.00" data-brotinho-price="19.25">
                            <input type="checkbox" id="brotinhoDocePecado"> <label for="brotinhoDocePecado" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                        <div class="item-selection">
                            <label for="qtyRomeuJulieta">8. Romeu e Julieta (R$43,00 / Brotinho R$15,05)</label>
                            <input type="number" id="qtyRomeuJulieta" min="0" value="0" data-price="43.00" data-brotinho-price="15.05">
                            <input type="checkbox" id="brotinhoRomeuJulieta"> <label for="brotinhoRomeuJulieta" style="flex: none; margin-left: 5px;">Brotinho</label>
                        </div>
                    </div>

                    <div class="borda-selection-group">
                        <h4>Bordas Recheadas (Taxa Extra)</h4>
                        <div class="item-selection">
                            <input type="checkbox" id="bordaCheddar" data-price="9.50">
                            <label for="bordaCheddar">Borda Cheddar (R$9,50)</label>
                            <input type="number" id="qtyBordaCheddar" min="0" value="0" style="display: none;">
                        </div>
                        <div class="item-selection">
                            <input type="checkbox" id="bordaCatupiry" data-price="11.50">
                            <label for="bordaCatupiry">Borda Catupiry (R$11,50)</label>
                            <input type="number" id="qtyBordaCatupiry" min="0" value="0" style="display: none;">
                        </div>
                        <div class="item-selection">
                            <input type="checkbox" id="bordaChocolate" data-price="14.50">
                            <label for="bordaChocolate">Borda Chocolate ao Leite (R$14,50)</label>
                            <input type="number" id="qtyBordaChocolate" min="0" value="0" style="display: none;">
                        </div>
                        <div class="item-selection">
                            <input type="checkbox" id="bordaRequeijao" data-price="13.50">
                            <label for="bordaRequeijao">Borda Requeijão (R$13,50)</label>
                            <input type="number" id="qtyBordaRequeijao" min="0" value="0" style="display: none;">
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="deliveryMethod">Forma de Entrega:</label>
                        <select id="deliveryMethod">
                            <option value="retirada">Retirada no Local</option>
                            <option value="delivery">Via Delivery (Taxa R$5,00)</option>
                        </select>
                    </div>

                    <button type="submit">Finalizar Pedido</button>
                </form>

                <div id="orderSummary" class="container">
                    <h4>Resumo do Pedido</h4>
                    <p id="summaryDetails"></p>
                    <p>Total a pagar: <span id="totalPrice">R$0,00</span></p>
                    <p class="highlight-text">Pagamento via PIX. Chave PIX: <strong style="color: var(--color-primary);">66992115947</strong> (telefone).</p>
                    <p>Por favor, envie o comprovante de pagamento PIX junto ao pedido via WhatsApp. Seu pedido só será produzido mediante o comprovante.</p>
                    <p>Se o pagamento for feito em até <span class="highlight-text">15 minutos</span> após a solicitação do pedido, você receberá um desconto de <span class="highlight-text">R$1,00!</span></p>
                </div>
            </div>
        </section>

        <hr>

        <section id="contato">
            <div class="container">
                <h3>Entre em Contato</h3>
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fab fa-whatsapp"></i>
                        <h4>WhatsApp</h4>
                        <a href="https://wa.me/5566992115947" target="_blank">(66) 9 9211-5947</a>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <h4>E-mail</h4>
                        <a href="mailto:kakaupizzaria123@gmail.com">kakaupizzaria123@gmail.com</a>
                    </div>
                </div>

                <form action="mailto:kakaupizzaria123@gmail.com" method="post" enctype="text/plain">
                    <label for="nome">Nome Completo:</label>
                    <input type="text" id="nome" name="Nome" required>

                    <label for="assunto">Assunto:</label>
                    <input type="text" id="assunto" name="Assunto" required>

                    <label for="mensagem">Mensagem:</label>
                    <textarea id="mensagem" name="Mensagem" required></textarea>

                    <button type="submit">Enviar Mensagem</button>
                </form>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 Kakau Pizzas. Todos os direitos reservados.</p>
            <p>Siga-nos nas redes sociais:</p>
            <div>
                <a href="https://instagram.com/kakau_pizzas" target="_blank"><i class="fab fa-instagram"></i> @kakau_pizzas</a>
                <a href="mailto:kakaupizzaria123@gmail.com"><i class="fas fa-envelope"></i> kakaupizzaria123@gmail.com</a>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const welcomeModal = document.getElementById('welcomeModal');
            const mobileMenu = document.getElementById('mobile-menu');
            const navbarLinks = document.getElementById('navbar-links');
            const orderForm = document.getElementById('orderForm');
            const orderSummary = document.getElementById('orderSummary');
            const summaryDetails = document.getElementById('summaryDetails');
            const totalPriceSpan = document.getElementById('totalPrice');

            // Show modal on page load
            welcomeModal.style.display = 'flex';

            // Close modal on click anywhere
            welcomeModal.addEventListener('click', () => {
                welcomeModal.style.display = 'none';
            });

            // Mobile menu toggle
            mobileMenu.addEventListener('click', () => {
                navbarLinks.classList.toggle('active');
                mobileMenu.classList.toggle('active');
            });

            // Close mobile menu when a link is clicked
            navbarLinks.querySelectorAll('a').forEach(link => {
                link.addEventListener('click', () => {
                    if (navbarLinks.classList.contains('active')) {
                        navbarLinks.classList.remove('active');
                        mobileMenu.classList.remove('active');
                    }
                });
            });

            // Pizza selection logic
            const pizzaTypeRadios = document.querySelectorAll('input[name="pizzaType"]');
            const salgadaPizzasDiv = document.getElementById('salgadaPizzas');
            const docePizzasDiv = document.getElementById('docePizzas');
            
            // Função para resetar quantidades e checkboxes de brotinho
            const resetPizzaSelections = (div) => {
                div.querySelectorAll('input[type="number"]').forEach(input => input.value = 0);
                div.querySelectorAll('input[type="checkbox"]').forEach(input => input.checked = false);
            };

            pizzaTypeRadios.forEach(radio => {
                radio.addEventListener('change', () => {
                    const selectedType = document.querySelector('input[name="pizzaType"]:checked').value;
                    if (selectedType === 'salgada') {
                        salgadaPizzasDiv.style.display = 'block';
                        docePizzasDiv.style.display = 'none';
                        resetPizzaSelections(docePizzasDiv);
                    } else if (selectedType === 'doce') {
                        salgadaPizzasDiv.style.display = 'none';
                        docePizzasDiv.style.display = 'block';
                        resetPizzaSelections(salgadaPizzasDiv);
                    } else { // ambas
                        salgadaPizzasDiv.style.display = 'block';
                        docePizzasDiv.style.display = 'block';
                    }
                });
            });

            // Borda selection logic
            const bordaCheckboxes = document.querySelectorAll('.borda-selection-group input[type="checkbox"]');
            bordaCheckboxes.forEach(checkbox => {
                checkbox.addEventListener('change', (event) => {
                    // Assume the quantity input is the second sibling after the label for direct access
                    const qtyInput = event.target.nextElementSibling.nextElementSibling; 
                    if (qtyInput && qtyInput.type === 'number') { // Ensure it's the quantity input
                        if (event.target.checked) {
                            qtyInput.style.display = 'inline-block';
                            qtyInput.value = 1; // Default to 1 when checked
                        } else {
                            qtyInput.style.display = 'none';
                            qtyInput.value = 0; // Reset quantity when unchecked
                        }
                    }
                });
            });


            orderForm.addEventListener('submit', (event) => {
                event.preventDefault();

                let total = 0;
                let orderDetails = [];
                let hasBrotinho = false;
                let numPizzas = 0;

                // Pizzas Salgadas
                const pizzasSalgadas = [
                    { id: 'qtyMussarela', name: 'Mussarela Tradicional', price: 55.00, brotinhoPrice: 19.25, brotinhoId: 'brotinhoMussarela' },
                    { id: 'qtyCalabresa', name: 'Calabresa', price: 60.00, brotinhoPrice: 21.00, brotinhoId: 'brotinhoCalabresa' },
                    { id: 'qtyPresunto', name: 'Presunto e Queijo', price: 58.00, brotinhoPrice: 20.30, brotinhoId: 'brotinhoPresunto' },
                    { id: 'qtyVegetariano', name: 'Vegetariano de Legumes', price: 60.00, brotinhoPrice: 21.00, brotinhoId: 'brotinhoVegetariano' },
                    { id: 'qtyPortuguesa', name: 'Portuguesa', price: 67.00, brotinhoPrice: 23.45, brotinhoId: 'brotinhoPortuguesa' }
                ];

                // Pizzas Doces
                const pizzasDoces = [
                    { id: 'qtyChocolate', name: 'Chocolate', price: 45.00, brotinhoPrice: 15.75, brotinhoId: 'brotinhoChocolate' },
                    { id: 'qtyDocePecado', name: 'Doce Pecado', price: 55.00, brotinhoPrice: 19.25, brotinhoId: 'brotinhoDocePecado' },
                    { id: 'qtyRomeuJulieta', name: 'Romeu e Julieta', price: 43.00, brotinhoPrice: 15.05, brotinhoId: 'brotinhoRomeuJulieta' }
                ];

                const allPizzas = [...pizzasSalgadas, ...pizzasDoces];

                allPizzas.forEach(pizza => {
                    const qtyInput = document.getElementById(pizza.id);
                    const brotinhoCheckbox = document.getElementById(pizza.brotinhoId);
                    const quantity = parseInt(qtyInput.value);

                    if (quantity > 0) {
                        numPizzas += quantity;
                        let itemPrice = 0;
                        let itemName = pizza.name;
                        if (brotinhoCheckbox && brotinhoCheckbox.checked) {
                            itemPrice = pizza.brotinhoPrice;
                            itemName += ' (Brotinho)';
                            hasBrotinho = true;
                        } else {
                            itemPrice = pizza.price;
                        }
                        total += quantity * itemPrice;
                        orderDetails.push(`${quantity}x ${itemName} (R$${(quantity * itemPrice).toFixed(2).replace('.', ',')})`);
                    }
                });

                // Bônus Brotinho Doce na compra de 3 pizzas
                let brotinhoBonusText = "";
                if (numPizzas >= 3) {
                    brotinhoBonusText = "\n*** GANHE UM BROTINHO DOCE NO SABOR QUE DESEJAR! ***";
                }


                // Bordas Recheadas
                const bordas = [
                    { id: 'bordaCheddar', name: 'Borda Cheddar', price: 9.50 },
                    { id: 'bordaCatupiry', name: 'Borda Catupiry', price: 11.50 },
                    { id: 'bordaChocolate', name: 'Borda Chocolate ao Leite', price: 14.50 },
                    { id: 'bordaRequeijao', name: 'Borda Requeijão', price: 13.50 }
                ];

                bordas.forEach(borda => {
                    const bordaCheckbox = document.getElementById(borda.id);
                    // Construct the ID for the quantity input (e.g., 'qtyBordaCheddar' for 'bordaCheddar')
                    const qtyBordaInputId = 'qty' + borda.id.charAt(0).toUpperCase() + borda.id.slice(1);
                    const qtyBordaInput = document.getElementById(qtyBordaInputId);
                    
                    if (bordaCheckbox.checked && qtyBordaInput && parseInt(qtyBordaInput.value) > 0) {
                        let bordaPrice = borda.price;
                        // Apply half price for brotinho if *any* brotinho was selected in the order
                        if (hasBrotinho) { 
                            bordaPrice /= 2;
                        }
                        const qtyBorda = parseInt(qtyBordaInput.value);
                        total += qtyBorda * bordaPrice;
                        orderDetails.push(`${qtyBorda}x ${borda.name} (R$${(qtyBorda * bordaPrice).toFixed(2).replace('.', ',')})`);
                    }
                });

                // Forma de Entrega
                const deliveryMethod = document.getElementById('deliveryMethod').value;
                let deliveryCost = 0;
                let deliveryText = "Retirada no Local";
                if (deliveryMethod === 'delivery') {
                    deliveryCost = 5.00;
                    total += deliveryCost;
                    deliveryText = "Via Delivery";
                    orderDetails.push(`Taxa de Entrega: R$${deliveryCost.toFixed(2).replace('.', ',')}`);
                }

                // Desconto de 1 real por pagamento em 15 minutos
                let discountText = "";
                let discountAmount = 0;
                // Para simulação, vamos aplicar o desconto. Em um cenário real, isso exigiria um backend para controle de tempo.
                discountAmount = 1.00;
                total -= discountAmount;
                discountText = `Desconto de R$${discountAmount.toFixed(2).replace('.', ',')} (Pagamento em 15 minutos)`;
                orderDetails.push(discountText);
                

                const finalTotal = total.toFixed(2);
                totalPriceSpan.textContent = `R$${finalTotal.replace('.', ',')}`;
                summaryDetails.innerHTML = orderDetails.join('<br>');
                orderSummary.style.display = 'block';

                // WhatsApp message generation
                const now = new Date();
                const orderDate = now.toLocaleDateString('pt-BR');
                const orderTime = now.toLocaleTimeString('pt-BR', { hour: '2-digit', minute: '2-digit' });

                let whatsappMessage = `Olá Kakau Pizzas!\n\nMeu pedido:\n`;
                whatsappMessage += orderDetails.map(item => `- ${item}`).join('\n');
                whatsappMessage += `\n\nForma de Entrega: ${deliveryText}`;
                whatsappMessage += `\nValor Total: R$${finalTotal.replace('.', ',')}`;
                whatsappMessage += `\n\nData do Pedido: ${orderDate}`;
                whatsappMessage += `\nHorário do Pedido: ${orderTime}`;
                whatsappMessage += brotinhoBonusText; // Adiciona o texto do bônus
                whatsappMessage += `\n\nChave PIX para pagamento: 66992115947 (telefone).`;
                whatsappMessage += `\nPor favor, envie o comprovante de pagamento PIX para que o pedido seja produzido.`;
                whatsappMessage += `\nLembre-se do seu desconto de R$${discountAmount.toFixed(2).replace('.', ',')} se o pagamento for feito em 15 minutos!`;


                const whatsappUrl = `https://wa.me/5566992115947?text=${encodeURIComponent(whatsappMessage)}`;
                window.open(whatsappUrl, '_blank');

                alert("Pedido enviado! A sua pizza será produzida mediante comprovante de pagamento PIX.");
            });
        });
    </script>
</body>
</html>
