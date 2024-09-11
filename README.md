# Fina - Aplicação de Controle Financeiro

Fina é uma aplicação de controle financeiro desenvolvida para ajudar usuários a gerenciar suas finanças de forma eficiente. O sistema é dividido em três partes principais, cada uma com uma responsabilidade bem definida:

1. **Fina.API**: API feita com .NET Minimal APIs.
2. **Fina.Web**: Frontend desenvolvido com Blazor, utilizando a biblioteca de componentes MudBlazor.
3. **Fina.Core**: Biblioteca de classes que realiza a comunicação entre a API e o frontend, além de organizar as regras de negócio da aplicação.

## Estrutura do Projeto

O projeto foi dividido em três subprojetos:

### 1. Fina.API
A API minimalista desenvolvida com .NET permite operações CRUD relacionadas ao controle financeiro. Ela expõe endpoints para interação com o frontend e realiza a persistência dos dados.

- **Tecnologias utilizadas**:
  - .NET 8 (Minimal APIs)
  - Entity Framework Core
  - SQL Server 
  - Swagger para documentação

### 2. Fina.Web
A interface de usuário (UI) foi criada com Blazor e utiliza a biblioteca MudBlazor para fornecer uma experiência de usuário moderna e responsiva.

- **Tecnologias utilizadas**:
  - Blazor WebAssembly
  - MudBlazor (biblioteca de componentes)
  - HTML5 e CSS3 para estilização

### 3. Fina.Core
A biblioteca Fina.Core contém as classes responsáveis pelas regras de negócio e a comunicação entre a API e o frontend. Também promove a separação de responsabilidades e facilita a manutenção do código.

- **Tecnologias utilizadas**:
  - Data Models e ViewModels para compartilhar dados entre API e Web
  - Serviços para manipulação de dados e validações

## Funcionalidades Principais

- Cadastro de despesas e receitas
- Categorização de transações financeiras
- Visualização de saldo e relatórios financeiros
- Edição e exclusão de registros
- Responsividade para dispositivos móveis

## Como Executar a Aplicação

### Requisitos:

- .NET 8 SDK ou superior
- Visual Studio ou VS Code

### Executando a API:

1. Clone o repositório:
    ```bash
    git clone https://github.com/BernardoMeine/fina.git
    ```
2. Navegue até a pasta `Fina.API`:
    ```bash
    cd Fina/Fina.API
    ```
3. Restaure os pacotes e execute a aplicação:
    ```bash
    dotnet restore
    dotnet run
    ```

A API estará disponível em `https://localhost:5001`.

### Executando o Web:

1. Navegue até a pasta `Fina.Web`:
    ```bash
    cd ../Fina.Web
    ```
2. Restaure os pacotes e execute o frontend:
    ```bash
    dotnet restore
    dotnet run
