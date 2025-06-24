# Tarefas App

Este projeto é uma aplicação web desenvolvida em .NET 8.0 que permite gerenciar tarefas. A aplicação oferece funcionalidades para cadastrar, editar e excluir tarefas em uma única tabela no banco de dados.

## Estrutura do Projeto

A estrutura do projeto é a seguinte:

```
tarefas-app
├── Controllers
│   └── TarefasController.cs       # Controlador para gerenciar operações de CRUD para tarefas
├── Models
│   └── Tarefa.cs                  # Modelo que representa a entidade de tarefa
├── Data
│   └── AppDbContext.cs            # Contexto do banco de dados
├── Views
│   └── Tarefas
│       ├── Index.cshtml           # View para listar tarefas
│       ├── Create.cshtml          # View para criar uma nova tarefa
│       ├── Edit.cshtml            # View para editar uma tarefa existente
│       └── Delete.cshtml          # View para confirmar a exclusão de uma tarefa
├── wwwroot
│   └── css
│       └── site.css               # Estilos para as views da aplicação
├── appsettings.json               # Configurações da aplicação
├── Program.cs                     # Ponto de entrada da aplicação
└── Startup.cs                     # Configuração dos serviços e middleware
```

## Instruções para Configuração e Execução

1. **Clone o repositório**:
   ```
   git clone <URL do repositório>
   cd tarefas-app
   ```

2. **Instale as dependências**:
   Certifique-se de ter o .NET 8.0 instalado e execute:
   ```
   dotnet restore
   ```

3. **Configure a string de conexão**:
   Edite o arquivo `appsettings.json` para configurar a string de conexão com seu banco de dados.

4. **Crie o banco de dados**:
   Execute as migrações para criar o banco de dados:
   ```
   dotnet ef database update
   ```

5. **Execute a aplicação**:
   Inicie a aplicação com o comando:
   ```
   dotnet run
   ```

6. **Acesse a aplicação**:
   Abra um navegador e vá para `http://localhost:5000` para acessar a aplicação.

## Funcionalidades

- **Cadastrar Tarefas**: Permite adicionar novas tarefas ao banco de dados.
- **Editar Tarefas**: Permite modificar tarefas existentes.
- **Excluir Tarefas**: Permite remover tarefas do banco de dados.
- **Listar Tarefas**: Exibe todas as tarefas cadastradas em uma tabela.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.