# RestWithASPNET - API REST em .NET 8

Este projeto é uma Web API robusta desenvolvida em C# para o estudo de arquitetura REST, injeção de dependência e padrões de desenvolvimento no ecossistema .NET. O desenvolvimento foi realizado em ambiente **Debian Linux** utilizando **Sublime Text**.

## 🛠️ Tecnologias e Ferramentas

* **Framework:** .NET 8
* **Linguagem:** C#
* **Ambiente:** Debian 13 (Trixie)
* **Editor:** Sublime Text 4
* **Documentação:** Swagger / OpenAPI
* **Testes de API:** Bruno

## 📌 Funcionalidades

### 1. Calculadora (CalculatorController)
Endpoints para operações matemáticas básicas e avançadas através de parâmetros de rota:
* **Soma:** `GET /calculator/sum/{num1}/{num2}`
* **Raiz Quadrada:** `GET /calculator/square-root/{num}`
* **Validação:** Implementa lógica para garantir que apenas entradas numéricas sejam processadas.

### 2. Gestão de Pessoas (PersonController)
Implementação de um CRUD completo utilizando o padrão de camadas (Controller -> Service -> Model):
* `GET /api/person`: Lista todas as pessoas (Mock).
* `GET /api/person/{id}`: Busca uma pessoa por ID.
* `POST /api/person`: Cria uma nova pessoa.
* `PUT /api/person`: Atualiza dados de uma pessoa.
* `DELETE /api/person/{id}`: Remove uma pessoa do sistema.

---

## 📂 Estrutura do Projeto

* **Controllers/**: Lida com as requisições HTTP e rotas.
* **Model/**: Define a estrutura da entidade `Person`.
* **Services/**: Contém a lógica de negócio e interfaces (`IPersonService`).
* **Properties/**: Configurações de execução como o `launchSettings.json`.

---

## 🚀 Como Executar

1. **Compilar e rodar:**
   Abra o terminal na pasta raiz do projeto e execute:
   ```bash
   dotnet run
