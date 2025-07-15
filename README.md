# Petinder 🐾

Sistema web para adoção de animais domésticos desenvolvido com Node.js, Express e TypeScript. O projeto permite visualizar e buscar pets disponíveis para adoção, categorizados por espécie.

## Funcionalidades

- **Catálogo de Pets**: Visualização de todos os animais disponíveis para adoção
- **Filtros por Espécie**: Navegação separada para cães, gatos e peixes
- **Sistema de Busca**: Pesquisa de animais por raça
- **Interface Responsiva**: Design adaptável para diferentes dispositivos
- **Informações Detalhadas**: Exibição de nome, cor e gênero de cada pet

## Tecnologias Utilizadas

- **Node.js** - Ambiente de execução JavaScript
- **Express** - Framework web para Node.js
- **TypeScript** - Superset tipado do JavaScript
- **Mustache** - Template engine para renderização de views
- **CSS3** - Estilização da interface

## Pré-requisitos

Antes de começar, você precisa ter instalado em sua máquina:
- [Node.js](https://nodejs.org/) (versão 14 ou superior)
- [npm](https://www.npmjs.com/) ou [yarn](https://yarnpkg.com/)

### Pré-requisitos globais:

```bash
npm i -g nodemon typescript ts-node
```

## Instalação

1. Clone o repositório
```bash
git clone https://github.com/ItamarJuniorDEV/node-ts-petinder.git
cd node-ts-petinder
```

2. Instale as dependências
```bash
npm install
```

3. Configure as variáveis de ambiente
```bash
# Crie um arquivo .env na raiz do projeto
cp .env.example .env
```

4. Configure a porta no arquivo `.env`
```env
PORT=3000
```

## Como Executar

### Modo de desenvolvimento
```bash
npm run start-dev
```

### Modo de produção
```bash
npm run build
npm start
```

O servidor estará rodando em `http://localhost:3000` (ou na porta configurada no .env)

## Estrutura do Projeto

```
node-ts-petinder/
├── public/
│   ├── css/
│   │   └── style.css
│   └── images/
├── src/
│   ├── controllers/
│   │   ├── pageController.ts
│   │   └── searchController.ts
│   ├── helpers/
│   │   └── createMenuObject.ts
│   ├── models/
│   │   └── pet.ts
│   ├── routes/
│   │   └── index.ts
│   ├── views/
│   │   ├── pages/
│   │   │   ├── 404.mustache
│   │   │   └── page.mustache
│   │   └── partials/
│   │       ├── footer.mustache
│   │       └── header.mustache
│   └── server.ts
├── .env
├── .gitignore
├── package-lock.json
├── package.json
├── README.md
└── tsconfig.json
```

## Rotas Disponíveis

- `GET /` - Página inicial (todos os animais)
- `GET /home` - Página inicial (todos os animais)
- `GET /dogs` - Listagem de cachorros
- `GET /cats` - Listagem de gatos
- `GET /fishes` - Listagem de peixes
- `GET /search?q=` - Busca por raça

## Tipos de Pets Disponíveis

### Cachorros
- Pastor-alemão
- Labrador-retriever
- Zwergspitz
- Husky Siberiano
- Golden Retriever
- Poodle
- Bulldog

### Gatos
- Persa
- Maine Coon
- Bengal
- Siamês
- Sphynx

### Peixes
- Tetra Neon
- Mato Grosso
- Limpa Vidro
- Tanictis
- Acará Bandeira

## Como Contribuir

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## Autor

**Itamar Junior**

---

Se este projeto te ajudou, considere dar uma estrela!