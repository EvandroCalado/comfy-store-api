# E-commerce API com Strapi

Esta API foi desenvolvida utilizando o Strapi, um poderoso sistema de gerenciamento de conteúdo (CMS) que facilita a criação e administração de APIs robustas. A finalidade principal desta API é fornecer funcionalidades essenciais para um sistema de e-commerce, incluindo manipulação de produtos, processamento de pedidos e gestão de listas de desejos.

## Recursos Principais

### 1. Produtos (Products)

A API permite a criação, leitura, atualização e exclusão de produtos. Cada produto possui atributos como nome, descrição, preço, e estoque, proporcionando uma base sólida para a gestão do catálogo de produtos.

#### Exemplo de Endpoints:

- `GET /api/products`: Retorna a lista completa de produtos.
- `GET /api/products/:id`: Retorna os detalhes de um produto específico.

### 2. Pedidos (Orders)

A API oferece funcionalidades relacionadas ao processamento de pedidos. Os pedidos contêm informações sobre os produtos selecionados, o cliente, e o status atual do pedido.

#### Exemplo de Endpoints:

- `GET /api/orders`: Retorna a lista de todos os pedidos.
- `POST /api/orders`: Cria um novo pedido.
- `DELETE /api/orders/:id`: Remove o status de um pedido existente.

### 3. Lista de Desejos (Wishlist)

A API inclui recursos para gerenciar listas de desejos dos clientes. Os usuários podem adicionar produtos à lista de desejos para futuras referências.

#### Exemplo de Endpoints:

- `GET /api/wishlists/:userId`: Retorna a lista de desejos de um usuário específico.
- `POST /api/wishlists/:userId/:productId`: Adiciona um produto à lista de desejos de um usuário.
- `DELETE /api/wishlists/:wishlistId`: Remove um produto da lista de desejos de um usuário.

## Configuração

1. **Instalação do Strapi:**
   - Clone este repositório.
   - Execute `npm install ou yarn install` para instalar as dependências.
   - Configure o arquivo `.env` conforme necessário.

2. **Configuração do Banco de Dados:**
   - Configure as credenciais do banco de dados no arquivo `.env`.
   - Execute `npm run setup` para configurar o banco de dados.

3. **Iniciar o Servidor:**
   - Execute `npm run develop` para iniciar o servidor Strapi.

Agora, sua API estará disponível para integração com seu front-end de e-commerce.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) ou enviar pull requests para melhorar esta API de e-commerce desenvolvida com Strapi.

## Licença

Este projeto é licenciado sob a [Licença MIT](LICENSE).
