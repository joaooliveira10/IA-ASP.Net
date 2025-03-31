# Assistente de Ensino

Um aplicativo moderno de assistência educacional desenvolvido com ASP.NET Blazor, combinando tecnologias de IA para melhorar a experiência de aprendizado.


## 📋 Sumário

- [Visão Geral](#visão-geral)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Funcionalidades](#funcionalidades)
- [Requisitos do Sistema](#requisitos-do-sistema)
- [Instalação](#instalação)
- [Configuração](#configuração)
- [Estrutura do Projeto](#estrutura-do-projeto)

## 🔍 Visão Geral

O **Assistente de Ensino** é uma plataforma educacional que utiliza inteligência artificial para facilitar o processo de aprendizagem. Desenvolvido com ASP.NET Blazor, o aplicativo oferece uma experiência interativa para estudantes e educadores, com recursos modernos de player de conteúdo e integração com tecnologias de IA.

## 💻 Tecnologias Utilizadas

- **Frontend**: Blazor WebAssembly
- **Backend**: ASP.NET Core 8.0
- **Banco de Dados**: SQLite
- **Estilo**: CSS/Bootstrap
- **Integração de IA**: OpenIA ChatGPT Api


## ✨ Funcionalidades

- **Player de Conteúdo**: Reprodução de material educacional com controles avançados
- **Integração com IA**: Assistência inteligente e personalizada
- **Interface Responsiva**: Acessível em dispositivos móveis e desktop
- **Gerenciamento de Conteúdo**: Organização eficiente de materiais educacionais
- **Painel Administrativo**: Para educadores gerenciarem recursos e conteúdos

## 🖥️ Requisitos do Sistema

- .NET 8.0 SDK ou superior
- Node.js e npm (para desenvolvimento frontend)
- Navegador moderno com suporte a WebAssembly
- Git (para controle de versão)

## 🚀 Instalação

Siga estas etapas para configurar o ambiente de desenvolvimento:

1. **Clone o repositório**
    ```bash
    git clone https://github.com/joaooliveira10/IA-ASP.Net.git
    cd IA-ASP.Net
    ```

2. **Restaure as dependências**
    ```bash
    dotnet restore
    ```

3. **Configure o banco de dados**
    ```bash
    cd src/AssistenteDeEnsino
    dotnet ef database update
    ```

4. **Execute o aplicativo**
    ```bash
    dotnet run
    ```

5. **Acesse o aplicativo**
    Abra seu navegador e navegue para `https://localhost:7227` ou conforme indicado no console.

## ⚙️ Configuração

### Configurações do Banco de Dados

O arquivo `appsettings.json` contém configurações para conexão com o banco de dados:

```json
"ConnectionStrings": {
  "DefaultConnection": "Data Source=AssistenteDeEstudos.db"
}
```

### Configurações da IA

Para configurar a integração com serviços de IA, adicione suas chaves de API ao arquivo `appsettings.json`:

```json
"AIServices": {
  "ApiKey": "sua-chave-api-aqui",
  "Endpoint": "https://api.servico-ia.com"
}
```

## 📁 Estrutura do Projeto

```
src/
├── AssistenteDeEnsino/              # Aplicação principal (Server)
│   ├── Components/                  # Componentes Blazor
│   │   ├── Layout/                  # Layouts da aplicação
│   │   ├── Pages/                   # Páginas da aplicação
│   │   └── Player/                  # Componente de reprodução de conteúdo
│   ├── Configurations/              # Configurações da aplicação
│   ├── Data/                        # Camada de acesso a dados
│   ├── Migrations/                  # Migrações do Entity Framework
│   ├── Services/                    # Serviços da aplicação
│   └── wwwroot/                     # Recursos estáticos
├── AssistenteDeEnsino.Client/       # Cliente Blazor WebAssembly
     ├── Pages/                       # Páginas do cliente
     └── wwwroot/                     # Recursos estáticos do cliente
```

