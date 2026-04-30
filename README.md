# 🕹️ Pokédex - Agenda Pokémon

Este projeto consiste em um sistema **CRUD completo** (Create, Read, Update, Delete) para o gerenciamento de Pokémon, desenvolvido como parte da disciplina **DS151 - Desenvolvimento para Dispositivos Móveis**. O sistema é composto por um aplicativo Android nativo e uma API de suporte integrada a um banco de dados na nuvem.

## 📋 Sobre o Projeto
O **Centro de Pesquisa Pokémon (CPP)** solicitou esta ferramenta para permitir que treinadores cadastrem novas descobertas, consultem estatísticas e organizem sua agenda de Pokémons de forma eficiente.

## ✨ Funcionalidades do Aplicativo

*   **SplashScreen:** Tela de apresentação exibida por 3 segundos ao iniciar o app.
*   **Autenticação:** Sistema de login com validação via API e banco de dados.
*   **Dashboard de Indicadores:** 
    *   Contador total de Pokémon cadastrados.
    *   Exibição dos Top 3 tipos e Top 3 habilidades mais frequentes.
*   **Gestão de Pokémon (CRUD):**
    *   **Cadastro:** Registro de nome, tipo e habilidades (1 a 3), com validação para evitar duplicidade de nomes.
    *   **Listagem:** Visualização de todos os Pokémon salvos no servidor.
    *   **Edição/Exclusão:** Alteração de detalhes ou remoção definitiva de registros através da tela de detalhes.
*   **Busca Avançada:**
    *   Pesquisa por **Tipo** com suporte a filtros parciais.
    *   Pesquisa por **Habilidade** individual.

## 🛠️ Tecnologias e Requisitos Técnicos

| Componente | Tecnologia / Especificação |
| :--- | :--- |
| **Linguagem** | Kotlin |
| **Plataforma** | Android (API 28) |
| **Backend** | API Web com integração a Banco de Dados na nuvem |
| **Comunicação** | Serviços Web para autenticação e persistência de dados |

## 📂 Estrutura de Atividades (Activities)

1.  **Login:** Captura credenciais e exibe `AlertDialog` em caso de falha.
2.  **Dashboard:** Activity principal com indicadores e menu de navegação.
3.  **Cadastro:** Formulário com validação de campos e upload para o servidor.
4.  **Lista Geral:** Exibe nomes dos Pokémon; ao clicar, direciona para Detalhes.
5.  **Detalhes:** Mostra todas as informações do Pokémon (exceto ID) e permite edição ou exclusão.
6.  **Busca por Tipo/Habilidade:** Filtra e lista resultados baseados na entrada do usuário.

## 🚀 Como Executar

> [!IMPORTANT]
> Certifique-se de que o backend está rodando e acessível pelo emulador/dispositivo Android.

1.  Clone este repositório.
2.  Abra o projeto no **Android Studio**.
3.  Certifique-se de que o SDK configurado é a **API 28**.
4.  Execute o aplicativo no emulador ou dispositivo físico.
5.  Para testes de login, utilize um dos 3 usuários pré-cadastrados no banco de dados.
