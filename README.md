# 🛒 Flask E-commerce API

Este é um projeto de API REST para um sistema de e-commerce simples, construído com **Flask**, **SQLAlchemy**, **Flask-Login** e **SQLite**.

## 🚧 Status do Projeto

> Em desenvolvimento 🚀  
Funcionalidades básicas de autenticação e CRUD de produtos já implementadas.

---

## 📦 Funcionalidades

- [x] Cadastro de usuários (via banco de dados diretamente)
- [x] Login e logout de usuários com `Flask-Login`
- [x] Adição, atualização, listagem e remoção de produtos (com autenticação)
- [x] CORS habilitado para integração com frontend
- [ ] Interface gráfica (em desenvolvimento)
- [ ] Cadastro e gerenciamento de usuários via API

---

## 🛠 Tecnologias Utilizadas

- [Flask](https://flask.palletsprojects.com/)
- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/)
- [Flask-Login](https://flask-login.readthedocs.io/)
- [SQLite](https://www.sqlite.org/index.html)
- [Flask-CORS](https://flask-cors.readthedocs.io/en/latest/)

---

## 🔐 Rotas de Autenticação

- `POST /login` – Realiza login com `username` e `password`
- `POST /logout` – Efetua logout do usuário autenticado

---

## 📦 Rotas de Produtos

> ⚠️ As rotas abaixo exigem autenticação (exceto listagem e detalhes)

- `GET /api/products` – Lista todos os produtos
- `GET /api/products/<id>` – Detalhes de um produto
- `POST /api/products/add` – Adiciona um novo produto
- `PUT /api/products/update/<id>` – Atualiza um produto existente
- `DELETE /api/products/delete/<id>` – Remove um produto

---
