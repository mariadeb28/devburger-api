<h1>DevBurger 🍔 API</h1>

Bem-vindo ao repositório da DevBurger API! Esta API foi desenvolvida para gerenciar pedidos e cardápios de um serviço de hambúrgueres. O projeto inclui funcionalidades de integração com a API do Stripe para processamento de pagamentos.

Índice
Visão Geral
Tecnologias Utilizadas
Instalação e Configuração
Rotas Disponíveis
Uso da API
Contribuição
Licença
Visão Geral
A DevBurger API foi criada para fornecer uma solução backend robusta que permite a criação, leitura, atualização e exclusão (CRUD) de itens do cardápio e pedidos, com integração de pagamento via Stripe.

Tecnologias Utilizadas
<br>
Node.js: Ambiente de execução do JavaScript no backend.
Express.js: Framework para criação de aplicações web.
Mongoose: ODM (Object Data Modeling) para MongoDB.
Stripe API: Integração para processar pagamentos.
Dotenv: Gerenciamento de variáveis de ambiente.
Instalação e Configuração
<br>

Clone o repositório:

bash
Copiar código
git clone https://github.com/mariadeb28/devburger-api.git
cd devburger-api
<br>

Instale as dependências:

bash
Copiar código
npm install
<br>
Crie um arquivo .env na raiz do projeto e defina as seguintes variáveis:

env
Copiar código
MONGO_URI=seu_mongo_uri
STRIPE_SECRET_KEY=sua_chave_secreta_stripe
PORT=porta_desejada (ex: 3000)
<br>
Inicie o servidor:

bash
Copiar código
<br>
npm start
<br>
Rotas Disponíveis
Produtos
GET /products: Retorna todos os produtos.
POST /products: Cria um novo produto.
GET /products/:id: Retorna um produto específico.
PUT /products/:id: Atualiza um produto existente.
DELETE /products/:id: Remove um produto.
<br>
Pedidos
GET /orders: Retorna todos os pedidos.
POST /orders: Cria um novo pedido.
GET /orders/:id: Retorna um pedido específico.
PUT /orders/:id: Atualiza um pedido existente.
DELETE /orders/:id: Remove um pedido.
<br>
Pagamentos
POST /payments: Processa um pagamento usando a integração com a API do Stripe.
<br>
Uso da API
Para interagir com a API, você pode usar ferramentas como Postman ou cURL para enviar requisições HTTP para as rotas mencionadas acima.

<br>
Exemplo de Requisição POST /products
json
Copiar código
{
  "name": "Classic Burger",
  "price": 12.99,
  "description": "Hambúrguer clássico com queijo, alface e tomate",
  "image": "url_da_imagem"
}
<br>
Contribuição
Sinta-se à vontade para contribuir com melhorias, relatórios de bugs ou novas ideias para funcionalidades. Faça um fork deste repositório, crie uma branch com suas alterações e envie um pull request.
