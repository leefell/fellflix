# Fellflix

## Descrição do Projeto
Fellflix é uma aplicação web que consome a API pública [The Movie Database (TMDb)](https://www.themoviedb.org/), permitindo aos usuários:

- Visualizar os 10 principais filmes em cartaz na página inicial.
- Acessar detalhes de filmes específicos, incluindo imagem, descrição, nome e opções para salvar nos favoritos ou assistir ao trailer no YouTube.
- Gerenciar uma lista de favoritos salva no **LocalStorage** do navegador.
- Navegar para páginas de erro ao acessar URLs inválidas.

É uma aplicação simples, desenvolvida com o objetivo de aprender e praticar conceitos de React, como `useState` e `useEffect`, além de integrar APIs públicas.

---

## Tecnologias Utilizadas
- **React** (v19.0.0)
- **React Router DOM** (v7.1.1)
- **Axios** (v1.7.9)
- **React Toastify** (v11.0.2)
- **gh-pages** (para deploy)

---

## Objetivo do Projeto
Estudar como consumir APIs públicas utilizando React, além de aprofundar os conhecimentos em hooks como `useState` e `useEffect`.

---

## Como Executar o Projeto

### Pré-requisitos
- Node.js instalado na máquina.

### Passos para execução
1. Clone este repositório.
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie o servidor de desenvolvimento:
   ```bash
   npm start
   ```
4. Acesse a aplicação no navegador através do endereço:
   [http://localhost:3000](http://localhost:3000).

### Deploy
O projeto está hospedado no GitHub Pages e pode ser acessado pelo link:
[Fellflix - GitHub Pages](https://leefell.github.io/fellflix).

---

## Estrutura do Projeto

```plaintext
Fellflix/
├── public/
│   ├── index.html
│   ├── robots.txt
├── src/
│   ├── components/
│   │   ├── Header/
│   │   │   ├── header.css
│   │   │   ├── index.js
│   ├── pages/
│   │   ├── Err/
│   │   ├── Favoritos/
│   │   ├── Filme/
│   │   ├── Home/
│   ├── services/
│   │   ├── api.js
│   ├── App.js
│   ├── index.css
│   ├── index.js
│   ├── routes.js
├── .env
├── .gitignore
├── LICENSE
├── package-lock.json
├── package.json
├── README.md
```

### Descrição dos Diretórios e Arquivos
- **public/**: Contém arquivos estáticos e o HTML base do projeto.
- **src/**: Contém todo o código-fonte.
  - **components/**: Componentes reutilizáveis, como o cabeçalho (Header).
  - **pages/**: Contém as páginas da aplicação, como Home, Favoritos, Filme e Err (página de erro).
  - **services/**: Gerencia chamadas à API externa usando Axios.
  - **App.js**: Componente principal da aplicação.
  - **routes.js**: Define as rotas da aplicação.
- **.env**: Variáveis de ambiente (se necessário).
- **package.json**: Gerencia dependências e scripts do projeto.
- **README.md**: Documentação inicial do projeto.

---

## Funcionalidades Principais
1. **Home**:
   - Exibe os 10 principais filmes em cartaz.
2. **Página de Filme**:
   - Exibe detalhes do filme, como imagem, descrição e nome.
   - Botões para salvar como favorito e assistir ao trailer (redireciona para o YouTube com uma pesquisa do tipo "[Nome do Filme] trailer").
3. **Favoritos**:
   - Exibe a lista de filmes favoritados, permitindo ver detalhes ou removê-los.
4. **Página de Erro**:
   - Exibida para URLs inválidas.

---

## Autor
**Alexandre Augusto dos Santos Feltrin**

- Este projeto foi inspirado em um curso online, adaptado e personalizado para estudos e práticas de desenvolvimento web.

---

## Observação
Fellflix é um projeto com fins apenas educacionais e utiliza a API pública do TMDb. Os direitos sobre os dados dos filmes pertencem à [The Movie Database](https://www.themoviedb.org/).
