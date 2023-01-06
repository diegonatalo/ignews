<h1 align="center">
  <img alt="Logo" src="assets/readme-banner.jpg" alt="Exemplo">
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg"/>
  <img src="https://img.shields.io/badge/commitizen-friendly-brightgreen.svg"/>
  <img src="https://img.shields.io/badge/license-MIT-blue" />
</p>

<h1 align="center">
    Ig.News
</h1>
<p align="center">Aplicação para inscrição de newsletter com pagamento via stripe</p>

<p align="center">
 <a href="#-sobre-o-projeto">Sobre o Projeto</a> •
 <a href="#-tecnologias">Tecnologias</a> •
 <a href="#-configurando-o-ambiente">Configurando o Ambiente</a> •
 <a href="#-licença">Licença</a>
</p>

## 📌 Sobre o projeto

O projeto tem como objetivo o estudo e desenvolvimento de uma aplicação em ReactJS com NextJS para listagem de posts e sistema de inscrição(subscription).
A aplicação foi desenvolvida utilizando o framework NextJS aplicando conceitos como consumo de API externas, API Root, Server Side Rendering (SSR), Static Site Generation (SSG), STRIPE para pagamentos das subscriptions, NextAuth para autenticação com Github, FaunaDB para armazenar as informações do usuário em um banco de dados e Prismic CMS para adição e gerenciamento do conteúdo dos posts.

---

## 💻 Tecnologias

- [ReactJS](https://reactjs.org/)
- [NextJS](https://nextjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [SASS](https://sass-lang.com/)
- [Next-Auth](https://next-auth.js.org/)
- [Stripe](https://stripe.com/)
- [FaunaDB](https://fauna.com/)
- [Prismic CMS](https://prismic.io/)

---

## 🌱 Configurando o ambiente

### 🚧 **Requisitos**

> Será necessário instalar os itens abaixo para clonar e executar o projeto corretamente!

- [Git](https://git-scm.com/)
- [Node](https://nodejs.org/)
- [Stripe CLI](https://stripe.com/docs/stripe-cli)

> Será necessário criar uma conta e configurar os seguintes serviços externos:

- [Stripe](https://stripe.com/)
- [FaunaDB](https://fauna.com/)
- [Prismic CMS](https://prismic.io/)

_Configurações dos serviços estão localizadas no arquivo servicesConfig.md na raiz do projeto._

### ⏩ **Clonando e executando a aplicação**

```bash
# Primeiro clone o repositório utilizando git:
$ git clone https://github.com/diegonatalo/exemplo.git

# Depois acesse a pasta do projeto:
$ cd exemplo

# Em seguida instale as dependências:
$ npm i

# Na raiz do projeto, crie uma copia do arquivo .env.local.example
# Altere o nome da copia para .env.local
# Preencha as variáveis ambiente de acordo com as instruções
$ cp .env.local.example .env.local

# Execute stripe listen para ouvir eventos do webhook
$ stripe listen --forward-to localhost:3000/api/webhooks

# Por fim, inicie a aplicação:
$ npm run dev
```

---

## 📜 Licença

Distribuído sob a licença MIT. Veja [LICENSE](LICENSE) para mais informações.

---

<p align="center">Feito com ❤️ por Deigo Natalo.</p>
