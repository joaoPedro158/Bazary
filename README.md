<!-- Coloque o link da imagem do seu banner aqui -->
<img src="https://via.placeholder.com/1500x500/FF2D20/FFFFFF?text=Bazary+-+E-commerce+Platform" alt="Bazary Banner" width="100%">

<h1 align="center">🛒 Bazary</h1>

<p align="center">
  Uma plataforma de e-commerce completa e funcional. Este projeto marca minha primeira experiência prática de desenvolvimento Full-Stack utilizando o framework Laravel.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

---

## 📸 Demonstração Visual

> **Nota:** Substitua os links das imagens abaixo pelos prints reais do seu projeto. Você pode arrastar as imagens diretamente para a caixa de edição do GitHub para gerar os links.

### Tela Inicial & Vitrine de Produtos
<img src="https://via.placeholder.com/800x450/eeeeee/999999?text=Print+da+Tela+Inicial+Aqui" alt="Tela Inicial do Bazary" width="100%">

### Carrinho de Compras & Checkout
<img src="https://via.placeholder.com/800x450/eeeeee/999999?text=Print+do+Carrinho+Aqui" alt="Carrinho de Compras" width="100%">

---

## ✨ Funcionalidades Principais

O sistema foi arquitetado utilizando boas práticas, separação de responsabilidades (Services, DTOs, Actions)[cite: 1] e conta com as seguintes funcionalidades:

* **Gestão de Usuários:** Autenticação, registro e gerenciamento de perfil seguros utilizando Laravel Jetstream e Fortify[cite: 1].
* **Catálogo de Produtos:** Visualização detalhada de produtos com controle de estoque e imagens[cite: 1].
* **Lista de Favoritos:** Os usuários podem favoritar produtos para compras futuras[cite: 1].
* **Carrinho de Compras:** Sistema completo de adição, remoção e atualização de itens no carrinho (`CarrinhoProduto` e `ItensCompra`)[cite: 1].
* **Gestão de Endereços:** Cadastro e seleção de múltiplos endereços de entrega por usuário[cite: 1].
* **Fluxo de Checkout e Pagamentos:** Integração de serviços para processamento de resumo de compras e pagamentos (`CheckoutService` e `PagamentoServiceImpl`)[cite: 1].
* **Painel Administrativo/Dashboard:** Área dedicada para visualização e gerenciamento[cite: 1].

---

## 🛠️ Arquitetura e Padrões

* **DTOs (Data Transfer Objects):** Utilizados para padronizar o tráfego de dados no fluxo de checkout e respostas de pagamento[cite: 1].
* **Services:** Lógica de negócios isolada em classes de serviço (ex: `CalculoService`, `RegistraCompraServiceImpl`) para manter os Controllers limpos[cite: 1].
* **Testes Automatizados:** Cobertura de testes de feature para autenticação, registro e fluxo de checkout (`CheckoutFlowTest`) usando PHPUnit[cite: 1].

---

## 🚀 Como Executar o Projeto Localmente

Siga o passo a passo abaixo para rodar o Bazary na sua máquina:

### Pré-requisitos
* PHP ^8.1
* Composer
* Node.js & NPM
* Banco de Dados (MySQL/PostgreSQL)
* Docker (Opcional, o projeto contém `Dockerfile` e arquivos de configuração)[cite: 1]

### 🚀 Como Executar o Projeto Localmente

1. **Instale as dependências do backend:**
```bash
   composer install
```

2. **Instale as dependências do frontend e gere os builds (Vite):**
```bash
   npm install
   npm run build
```

3. **Configure as variáveis de ambiente:**
   - Faça uma cópia do arquivo `.env.example` e renomeie para `.env`.
   - Configure as credenciais do seu banco de dados dentro do arquivo `.env`.

4. **Gere a chave da aplicação:**
```bash
   php artisan key:generate
```

5. **Rode as migrações e popule o banco (Seeders):**
```bash
   php artisan migrate --seed
```

6. **Inicie o servidor local:**
```bash
   php artisan serve
```

   O servidor estará rodando em `http://localhost:8000`.

---

### 👨‍💻 Autor

**João Pedro**

- 🌐 LinkedIn: [João Pedro](https://www.linkedin.com/in/joão-pedro-69384b335/)
- ✉️ E-mail: pjpedro150@gmail.com
