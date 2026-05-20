# HubCultural | Culturama 

O projeto Culturama é uma plataforma web interativa criada para conectar pessoas aos melhores eventos do Brasil. Centralizando a programação de festivais, exposições de arte, peças de teatro e conferências de tecnologia. Nesse projeto foi aplicado, na prática, a criação de um projeto com: Next.js 15, estruturação de rotas, layouts, otimizações e a migração de componentes React, resultando em uma aplicação ágil que facilita a descoberta de experiências incríveis.

## Funcionalidades

* **Exploração de Eventos:** Navegue por catálogos completos de eventos futuros e passados.
* **Filtro por Categorias:** Encontre rapidamente o que procura navegando por seções como Teatro, Música, Arte, Tecnologia e Festivais.
* **Busca Inteligente:** Pesquise eventos por título, descrição ou localização.
* **Detalhes do Evento:** Visualize datas, horários, localização, descrição completa e a organização do evento.
* **Interações do Usuário:** Adicione eventos aos seus favoritos ou compartilhe-os diretamente por meio da API nativa do navegador ou links diretos.

## Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

* **Framework:** Next.js (v15.5.4) com App Router.
* **Linguagem:** TypeScript.
* **Estilização:** Tailwind CSS.
* **Ícones:** Material UI Icons (`@mui/icons-material`).
* **Tipografia:** Fjalla One e Work Sans (via Google Fonts).
* **Backend/Mock API:** `json-server` para simulação de banco de dados REST.

## Como Executar o Projeto Localmente

Siga os passos abaixo para rodar o projeto na sua máquina:

1. **Clone o repositório:**
   ```bash
   git clone <url-do-repositorio>
   cd culturama
   ```
2. **Instale as dependências:**
   ```bash
   npm install
   ```
3. **Inicie a API Mockada (JSON Server):**
Para que os eventos e categorias sejam carregados na interface, é necessário rodar o servidor de dados na porta 3001.
   ```bash
   npm run server
   ```
4. **Inicie a Aplicação Frontend:**
Abra uma nova aba no seu terminal e inicie o servidor de desenvolvimento.
   ```bash
   npm run dev
   ```
5. **Acesse a plataforma:**
Abra http://localhost:3000 no seu navegador. A aplicação estará se comunicando automaticamente com a API em http://localhost:3001.

## Estrutura Principal do Projeto
* **`db.json`**: Banco de dados contendo os registros de eventos e categorias.
* **`@/hooks`**: Hooks customizados como `useEvents`, `useCategories` e `useSearch` que lidam com a lógica de dados e filtros.
* **`@/context`**: ContextAPI (`DataProvider`) centralizando as requisições HTTP e o estado global de eventos e categorias.
* **`@/layout/ui`**: Componentes reaproveitáveis de interface, como `Button`, `EventCard` e `CategoryCard`.
