# Requisitos do Projeto

## ⚙️ Requisitos Funcionais (RF)
- **RF01** – Permitir o cadastro de produtos (nome, preço, quantidade).
- **RF02** – Listar todos os produtos cadastrados.
- **RF03** – Adicionar produtos ao carrinho de compras.
- **RF04** – Remover produtos do carrinho de compras.
- **RF05** – Finalizar a compra, exibindo o valor total.

## 🛠️ Requisitos Não Funcionais (RNF)
- **RNF01** – A interface deve ser simples e intuitiva.
- **RNF02** – O código deve ser modular e organizado.
- **RNF03** – O sistema deve rodar em ambiente Windows ou Linux.
- **RNF04** – O repositório deve ser mantido no GitHub com versionamento.
- **RNF05** – Toda a documentação deve ser escrita em Markdown.

## 📊 Diagrama de Caso de Uso
Abaixo está o diagrama representando as interações do **Cliente** com o sistema:

```mermaid
usecaseDiagram
actor Cliente
Cliente --> (Cadastrar Produto)
Cliente --> (Listar Produtos)
Cliente --> (Adicionar ao Carrinho)
Cliente --> (Remover do Carrinho)
Cliente --> (Finalizar Compra)
