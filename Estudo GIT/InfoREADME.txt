Como Montar um README.md

Michael Douglas Bonfogo.

-------------------------------------------

Estrutura do README:

 Logo ou Banner
 Título e Descrição
 Badges
 Status do Projeto
 Tabela de Conteúdos
 Features
 Demonstração da Aplicação
 Pré-requisitos e como rodar a aplicação/testes
 Tecnologias utilizadas
 Contribuição
 Autor
 Licença

 -- Essa é uma sugestão de estrutura, cada um pode fazer conforme a necessidade do projeto. Vamos agora cobrir cada um dos tópicos da estrutura e outros pontos adicionais.

-------------------------------------------

 -- Logo ou Banner
  Status: Opcional

  Se seu projeto já tem uma logo adicione no README. Pode ser um banner também. Você pode criar uma logo ou banner usando o Canva.
  A logo ou banner podem substituir o título, mas não a descrição do projeto, veja um exemplo. O bom de manter o título e descrição em texto é que ajuda no SEO do Github, o Google vai ajudar indexar melhor seu projeto nas primeiras páginas de pesquisas, além de dar um resumo sobre o seu projeto.
  Exemplos de projetos com logo e banner.


-------------------------------------------

 -- Título e Descrição
  Status: Obrigatório

  Título: Nome curto do projeto
  Descrição: Uma breve descrição do objetivo do projeto.

   # Nome do Projeto 
   ou
   <h1 align="center">Nome do Projeto</h1>
        Nome do Projeto

  Com a descrição:

   ## Descrição do Projeto
   <p align="center">Escrever uma breve descrição</p>
   Escrever uma breve descrição

  <h1 align="center">
    <a href="https://pt-br.reactjs.org/">🔗 React</a>
  </h1>
  
  <p align="center">🚀 lib para construir interfaces do usuário com componentes reutilizáveis</p>
             🔗 React

  🚀 lib para construir interfaces do usuário com componentes reutilizáveis

-------------------------------------------
-- Badges
  Status: Opcional

  É uma questão de gosto pessoal e comunicação. As badges são úteis para indicar o status do projeto: você pode colocar a versão dele, link para licença, quantidade de issues, status da build, status dos testes.  Vale muito a pena colocar.
  As badges podem ficar no topo antes do título ou abaixo da descrição.
  Use o site shields.io para gerar suas badges.
  
  Você pode criar a sua própria badge:
  Os ícones de várias logos de produtos e tecnologias você encontra aqui: simpleicons.org.
  Podemos customizar partir da URL a abaixo:
  https://img.shields.io/static/v1?label=<LABEL>&message=<MESSAGE>&color=<COLOR>&style=<STYLE>&logo=<LOGO>
  
  Os parâmetros significam:   
   LABEL: texto do campo esquerdo
   MESSAGE: texto do campo direto
   COLOR: cor do campo direito, pode usar RGB.
   STYLE: estilo do badge inteiro. Podemos ter: plastic, flat, for-the-badge, social ou flat-square. Teste cada uma delas.
   LOGO: logo do campo esquerdo
   
  Como exemplo, vou escolher os seguintes parâmetros:
   LABEL: como Blog
   MESSAGE: como Rocketseat
   COLOR: 7159c1
   STYLE: como for-the-badge
   LOGO: como GHOST
   Podemos colocar ele no README assim em HTML:

<img src="https://img.shields.io/static/v1?label=Blog&message=Rocketseat&color=7159c1&style=for-the-badge&logo=ghost"/>
ou ainda em Markdown:

![Badge](https://img.shields.io/badge/Blog-Rocketseat-%237159c1?style=for-the-badge&logo=ghost)

-------------------------------------------

-- Tabela de Conteúdos
  Status: Obrigatório

  É ótimo colocar os índices de conteúdos, que é tabela onde a pessoa clica e vai para o tópico específico.
 Exemplo com markdown:

Tabela de conteúdos
=================
<!--ts-->
   * [Sobre](#Sobre)
   * [Tabela de Conteudo](#tabela-de-conteudo)
   * [Instalação](#instalacao)
   * [Como usar](#como-usar)
      * [Pre Requisitos](#pre-requisitos)
      * [Local files](#local-files)
      * [Remote files](#remote-files)
      * [Multiple files](#multiple-files)
      * [Combo](#combo)
   * [Tests](#testes)
   * [Tecnologias](#tecnologias)
<!--te-->

Tabela de conteúdos
 ° Sobre
 ° Tabela de Conteudo
 ° Instalação
 ° Como usar
  ° Pre Requisitos
  ° Local files
  ° Remote files
  ° Multiple files
  ° Combo
 ° Tests
 ° Tecnologias

 Se o README tiver poucos tópicos pode fazer inline, com HTML:

 <p align="center">
 <a href="#objetivo">Objetivo</a> •
 <a href="#roadmap">Roadmap</a> • 
 <a href="#tecnologias">Tecnologias</a> • 
 <a href="#contribuicao">Contribuição</a> • 
 <a href="#licenc-a">Licença</a> • 
 <a href="#autor">Autor</a>
</p>

Resultado:

Objetivo • Roadmap • Tecnologias • Contribuição • Licença • Autor

No README.md do Github você pode usar HTML o que ajuda muito.

-------------------------------------------

Status do Projeto
 Status: Obrigatório
 Indica se o projeto está em desenvolvimento ou já foi concluído.

<h4 align="center"> 
	🚧  React Select 🚀 Em construção...  🚧
</h4>

Resultado:
🚧 React Select 🚀 Em construção... 🚧

-------------------------------------------

-- Features
 Status: Opcional
 Você pode listar as funcionalidades da aplicação.
 É opcional, porém é muito importante colocar. Isso ajuda demais as pessoas entenderem o que já tem feito, se estiver em construção você vai checkando o que está pronto.

Exemplo:

### Features

- [x] Cadastro de usuário
- [x] Cadastro de cliente
- [ ] Cadastro de produtos

-- Demonstração da aplicação

-------------------------------------------

-- Demonstração da aplicação
  Status: Opcional
  
  Se for um projeto web e estiver hospedado em algum lugar, forneça o link. Se o deploy foi feito no Netlify tem um badge para isso.
  Se for uma API backend pode customizar um badge com um ícone do heroku. Pode também colocar o arquivo do Insomnia para ficar mais rápido para o usuário testar a API — Fica muito bom.
  Se a aplicação estiver em desenvolvimento, se for um app mobile ou website coloque os prints da tela ou um gif ilustrando a utilização.

  A maneira mais segura de manter os arquivos é criar uma pasta screenshots, github, assets, resources ou nome que você quiser e deixar os arquivos nela. Se você usar um CDN de imagens ou gif pode funcionar mas corre o risco do quebrar o link algum dia.
  Supondo que você tenha criado uma pasta assets no seu projeto e tem o arquivo banner.png, é assim que você pode adicionar a imagem:

  <h1 align="center">
  <img alt="NextLevelWeek" title="#NextLevelWeek" src="./assets/banner.png" />
</h1>

-------------------------------------------

-- Pré-requisitos e como rodar a aplicação/testes
  Status: Obrigatório

  Se o projeto for uma lib, você tem que mostrar os passos de como instalar e usar a lib, se for um projeto backend | web | mobile | desktop descreva os passos de como fazer para rodar na máquina.
  Se tiver testes é bom descrever como rodar os testes.

 Exemplo:

  ### Pré-requisitos

   Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
   [Git](https://git-scm.com), [Node.js](https://nodejs.org/en/). 
   Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/)

  ### 🎲 Rodando o Back End (servidor)

   ```bash
   # Clone este repositório
   $ git clone <https://github.com/tgmarinho/nlw1>

   # Acesse a pasta do projeto no terminal/cmd
   $ cd nlw1

   # Vá para a pasta server
   $ cd server

   # Instale as dependências
   $ npm install

   # Execute a aplicação em modo de desenvolvimento
   $ npm run dev:server

   # O servidor inciará na porta:3333 - acesse <http://localhost:3333>
```

Resultado:

 Pré-requisitos
 Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
 Git, Node.js.
 Além disto é bom ter um editor para trabalhar com o código como VSCode

 🎲 Rodando o Back End (servidor)
 # Clone este repositório
 $ git clone <https://github.com/tgmarinho/nlw1>

 # Acesse a pasta do projeto no terminal/cmd
 $ cd nlw1

 # Vá para a pasta server
 $ cd server

 # Instale as dependências
 $ npm install

 # Execute a aplicação em modo de desenvolvimento
 $ npm run dev:server

 # O servidor inciará na porta:3333 - acesse <http://localhost:3333> 

-------------------------------------------

-- Tecnologias utilizadas
 Status: Obrigatório para projetos de portfólio/estudos.
 Listar as tecnologias e colocar os links para o seus respectivos sites é um plus no README.

 ### 🛠 Tecnologias

 As seguintes ferramentas foram usadas na construção do projeto:

 - [Expo](https://expo.io/)
 - [Node.js](https://nodejs.org/en/)
 - [React](https://pt-br.reactjs.org/)
 - [React Native](https://reactnative.dev/)
 - [TypeScript](https://www.typescriptlang.org/)

Resultado:

Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:
 Expo
 Node.js
 React
 React Native
 ypeScript

-------------------------------------------

-- Contribuição
 Status: Opcional

 Se seu projeto começar a receber contribuições, uma maneira legal de reconhecer o trabalho dessas pessoas é adicionando na lista de contribuidores.
 Com certeza eles contribuíram porque gostam do projeto, e vão amar ♥️ receber esse esse reconhecimento.

-------------------------------------------

-- Autor
Status: Obrigatório

Aqui é interessante colocar seus contatos, redes sociais para as pessoas te encontrarem e começar um networking:

-------------------------------------------