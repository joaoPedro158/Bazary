
<h1 align="center">🛒 Bazary</h1>

<p align="center">
  Uma plataforma de e-commerce completa e funcional. Este projeto marca minha primeira experiência prática de desenvolvimento Full-Stack utilizando o framework Laravel.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

---

## 📸 Demonstração Visual

### Tela Inicial 
<img width="1910" height="1035" alt="pagina_principal" src="https://github.com/user-attachments/assets/d7f90660-72b0-41dc-8301-cfb8bb9184a6" />

### Carrinho de Compras & Checkout

<img width="1910" height="1392" alt="carrinho_compra" src="https://github.com/user-attachments/assets/7afb6af8-2881-42df-a0aa-79ccec9187a3" />
<img width="1910" height="1181" alt="seleciona_endereco" src="https://github.com/user-attachments/assets/5c115539-ec8d-493d-8c38-02d68277efe8" />


### Detalhe do Produto
<img width="1910" height="1241" alt="detalhe_produto" src="https://github.com/user-attachments/assets/b817e698-0244-4cab-86a4-5baaab455ad3" />

---

## ✨ Funcionalidades Principais

O sistema foi arquitetado utilizando boas práticas, separação de responsabilidades (Services, DTOs, Actions) e conta com as seguintes funcionalidades:

* **Gestão de Usuários:** Autenticação e registro  utilizando Laravel Jetstream e Fortify.
* **Catálogo de Produtos:** Visualização detalhada de produtos com controle de estoque e imagens.
* **Lista de Favoritos:** Os usuários podem favoritar produtos para compras futuras.
* **Carrinho de Compras:** Sistema completo de adição, remoção e atualização de itens no carrinho (`CarrinhoProduto` e `ItensCompra`).
* **Gestão de Endereços:** Cadastro e seleção de múltiplos endereços de entrega por usuário.
* **Fluxo de Checkout e Pagamentos:** Integração de serviços para processamento de resumo de compras e pagamentos (`CheckoutService` e `PagamentoServiceImpl`).
* **Painel Administrativo/Dashboard:** Pagina para gerencia os produtos cadastrado podendo apagar ou atualizar.

---

## 🛠️ Arquitetura e Padrões

* **Padrão MVC (Model-View-Controller):** A aplicação adota a arquitetura monolítica nativa do Laravel, estruturada de forma a garantir uma separação clara entre a interface do usuário (Views em Blade), o gerenciamento das requisições e regras de roteamento (Controllers) e a manipulação dos dados e regras de negócio (Models/Eloquent), resultando em um código mais organizado e de fácil manutenção.
* **Services:** Lógica de negócios isolada em classes de serviço (ex: `CalculoService`, `RegistraCompraServiceImpl`) para manter os Controllers limpos.
* **Testes Automatizados:** Cobertura de testes de feature para autenticação, registro e fluxo de checkout (`CheckoutFlowTest`) usando PHPUnit.

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
