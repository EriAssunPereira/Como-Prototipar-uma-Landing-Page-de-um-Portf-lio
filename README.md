# Como-Prototipar-uma-Landing-Page-de-um-Portfólio

Prototipar uma landing page de um portfólio utilizando o Figma é uma ótima maneira de visualizar e planejar o design antes de iniciar o desenvolvimento. Vou dividir o projeto em módulos e considerar a descrição fornecida.

### Módulos da Landing Page

1. **Cabeçalho (Header)**
   - Inclui o logotipo e a navegação.
   - Alinhado à esquerda para o logotipo e à direita para os itens de navegação.

   Exemplo de código HTML e CSS para o cabeçalho:

   ```html
   <header>
       <div class="logo">Meu Logo</div>
       <nav>
           <ul>
               <li><a href="#">Início</a></li>
               <li><a href="#">Portfólio</a></li>
               <li><a href="#">Sobre</a></li>
               <li><a href="#">Contato</a></li>
           </ul>
       </nav>
   </header>
   ```

   ```css
   header {
       display: flex;
       justify-content: space-between;
       align-items: center;
       padding: 20px;
   }

   .logo {
       font-size: 24px;
   }

   nav ul {
       list-style-type: none;
       padding: 0;
       margin: 0;
       display: flex;
   }

   nav ul li {
       margin-right: 20px;
   }

   nav ul li a {
       text-decoration: none;
       color: #333;
   }
   ```

2. **Seção de Destaque**
   - Destaque principal do portfólio.
   - Alinhado à esquerda para o texto e à direita para a imagem/ilustração.

   Exemplo de estrutura HTML e CSS para a seção de destaque:

   ```html
   <section class="destaque">
       <div class="texto">
           <h1>Meu Portfólio</h1>
           <p>Uma breve descrição do que faço e meus principais projetos.</p>
       </div>
       <div class="imagem">
           <img src="imagem-portfolio.jpg" alt="Imagem de destaque do portfólio">
       </div>
   </section>
   ```

   ```css
   .destaque {
       display: flex;
       justify-content: space-between;
       align-items: center;
       padding: 40px;
   }

   .texto {
       width: 50%;
       text-align: left;
   }

   .texto h1 {
       font-size: 36px;
       margin-bottom: 20px;
   }

   .texto p {
       font-size: 18px;
       line-height: 1.6;
   }

   .imagem {
       width: 40%;
       text-align: right;
   }

   .imagem img {
       max-width: 100%;
       height: auto;
   }
   ```

3. **Portfólio**
   - Grade de projetos ou trabalhos destacados.
   - Alinhado à esquerda para o título e à direita para os itens do portfólio.

   Exemplo de estrutura HTML e CSS para a seção de portfólio:

   ```html
   <section class="portfolio">
       <h2>Meus Projetos</h2>
       <div class="grid-projetos">
           <div class="projeto">
               <img src="projeto-1.jpg" alt="Projeto 1">
               <h3>Projeto 1</h3>
           </div>
           <div class="projeto">
               <img src="projeto-2.jpg" alt="Projeto 2">
               <h3>Projeto 2</h3>
           </div>
           <div class="projeto">
               <img src="projeto-3.jpg" alt="Projeto 3">
               <h3>Projeto 3</h3>
           </div>
       </div>
   </section>
   ```

   ```css
   .portfolio {
       padding: 40px;
   }

   .portfolio h2 {
       font-size: 24px;
       text-align: left;
   }

   .grid-projetos {
       display: grid;
       grid-template-columns: repeat(3, 1fr);
       gap: 20px;
       margin-top: 20px;
   }

   .projeto {
       text-align: center;
   }

   .projeto img {
       max-width: 100%;
       height: auto;
   }

   .projeto h3 {
       margin-top: 10px;
       font-size: 18px;
   }
   ```

4. **Rodapé (Footer)**
   - Informações de contato e links sociais.
   - Alinhado à esquerda para o texto de contato e à direita para os ícones de redes sociais.

   Exemplo de estrutura HTML e CSS para o rodapé:

   ```html
   <footer>
       <div class="contato">
           <p>Entre em contato: email@example.com</p>
       </div>
       <div class="redes-sociais">
           <a href="#"><i class="fab fa-facebook"></i></a>
           <a href="#"><i class="fab fa-twitter"></i></a>
           <a href="#"><i class="fab fa-instagram"></i></a>
       </div>
   </footer>
   ```

   ```css
   footer {
       display: flex;
       justify-content: space-between;
       align-items: center;
       padding: 20px;
       background-color: #f0f0f0;
   }

   .contato p {
       font-size: 14px;
       text-align: left;
   }

   .redes-sociais a {
       margin-left: 10px;
       font-size: 20px;
       color: #333;
   }
   ```

### Considerações Finais

Ao prototipar no Figma, podemos usar essas estruturas de HTML e CSS como referência para criar os diferentes componentes da landing page. O Figma permite arrastar e soltar elementos para montar o layout, definir tamanhos, cores, tipografia e interações, proporcionando uma visão clara de como a página final ficará antes de começar a codificação.
