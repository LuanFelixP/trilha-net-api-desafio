📌 DIO - Trilha .NET - API e Entity Framework

Este repositório contém a solução para o desafio de projeto do módulo de API e Entity Framework da DIO (Digital Innovation One)
.

🚀 Desafio de Projeto

O objetivo foi construir um sistema gerenciador de tarefas, permitindo o cadastro de uma lista de tarefas para organizar melhor a rotina do usuário.

A aplicação foi desenvolvida em .NET 6 Web API utilizando o Entity Framework Core para persistência de dados.

📖 Funcionalidades

O sistema permite realizar as operações básicas de um CRUD sobre tarefas:

✅ Criar uma tarefa

✅ Obter uma tarefa pelo ID

✅ Atualizar uma tarefa

✅ Deletar uma tarefa

✅ Listar todas as tarefas

✅ Consultar por Título

✅ Consultar por Data

✅ Consultar por Status

🛠️ Tecnologias Utilizadas

.NET 6

Entity Framework Core

Swagger
 (para documentação e testes de endpoints)

Banco de dados SQL Server LocalDB (padrão, mas pode ser alterado no appsettings.json)

🗂️ Estrutura da Tarefa (Model)
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}

🔗 Endpoints Disponíveis
Verbo	Endpoint	Parâmetro	Body
GET	/Tarefa/{id}	id	N/A
PUT	/Tarefa/{id}	id	Schema Tarefa
DELETE	/Tarefa/{id}	id	N/A
GET	/Tarefa/ObterTodos	N/A	N/A
GET	/Tarefa/ObterPorTitulo	titulo	N/A
GET	/Tarefa/ObterPorData	data	N/A
GET	/Tarefa/ObterPorStatus	status	N/A
POST	/Tarefa	N/A	Schema Tarefa
📌 Como Executar o Projeto

Clone este repositório:

git clone https://github.com/seu-usuario/dio-trilha-dotnet-api-ef.git


Acesse a pasta do projeto:

cd dio-trilha-dotnet-api-ef


Configure o banco de dados no arquivo appsettings.json (se necessário).

Execute as migrations para atualizar o banco de dados:

dotnet ef database update


Execute o projeto:

dotnet run


Acesse a documentação Swagger em:
👉 https://localhost:5001/swagger

📷 Imagens de Referência

Estrutura da classe Tarefa:


Documentação no Swagger:


📚 Aprendizados

Uso do Entity Framework Core para persistência.

Criação de endpoints REST com .NET 6.

Documentação automática com Swagger.

Implementação de consultas personalizadas.

✍️ Desenvolvido como parte da Trilha .NET - DIO.
