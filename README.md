# 📦 API de Produtos - Spring Boot

Este projeto consiste em uma API REST desenvolvida com **Spring Boot**, permitindo a gestão de produtos através de operações CRUD (Create, Read, Update, Delete). A API armazena os dados em um banco de dados relacional utilizando **Spring Data JPA**.

---

## 🚀 Tecnologias Utilizadas

- **Java 22**
- **Spring Boot**
- **Spring Data JPA**
- **SQlite Database** (ou outro banco configurado)
- **Spring Web**
- **Maven**

---

## 📂 Estrutura do Projeto

```plaintext
src/main/java  
├── com.produtoapi
│   ├── MeuProjetoSpringbootApplication.java
│   ├── controller
│   │   ├── ProdutoController.java
│   ├── model
│   │   ├── Produto.java
│   ├── repository
│   │   ├── ProdutoRepository.java
│   ├── service
│       ├── ProdutoService.java
```


## 🔧 Configuração do Projeto

### 📌 Pré-requisitos

Antes de começar, certifique-se de ter os seguintes itens instalados:

- **Java 22**
- **Maven**
- **Postman** (opcional, para testes)
- **Banco de Dados** 


## 📌 Endpoints da API

### 🔍 Listar Todos os Produtos
- **Método:** `GET`
- **URL:** `/produtos`
- **Retorno:** Lista de produtos cadastrados

---

### ➕ Criar um Novo Produto
- **Método:** `POST`
- **URL:** `/produtos`
- **Exemplo de Body (JSON):**
  ```json
  {
    "nome": "Notebook",
    "quantidade": 10,
    "preco": 3000.00,
    "status": "disponível"
  }

### 🔄 Atualizar um Produto
- **Método:** `PUT`
- **URL:** `/produtos/{id}`
- **Exemplo de Body (JSON):**

```json
{
"nome": "Notebook Gamer",
"quantidade": 5,
"preco": 4500.00,
"status": "disponível"
}
``` 
- `Retorno: Produto atualizado`

### ❌ Deletar um Produto
- **Método:** `DELETE`
- **URL:** `/produtos/{id}`
- **Retorno:** `Nenhum conteúdo (204)`

### 🔎 Buscar Produto por ID
- **Método:** `GET`
- **URL:** `/produtos/{id}`
- **Retorno:** `Produto correspondente ao ID informado`
