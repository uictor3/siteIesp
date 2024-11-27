# Site da Iesp

https://site-iesp.vercel.app/

O sistema foi criado na biblioteca react, o uso do React facilita muito em projetos que envolvem interfaces devido a seus componentes que torna mais fácil a reutilização e a manutenção do código, tornando o trabalho mais produtivo. 
Para a criação de um projeto React, no terminal do vscode põe o comando “npm create vite@latest”, se escolhe a linguagem na qual irá ser usada entre as opções que são apresentadas, no caso do site iesp foi a opção Javascript e logo após a escolha, dê um nome ao projeto e ao finalizar dê o comando “npm install”, o NPM (node package manager) é o gerenciador de pacotes do node.

O projeto Site Iesp está dividido em Packages:

data: Onde foi criado o db.json o database fake para que não fosse necessário a criação de um back durante os testes.

node modules: tem todos os arquivos que foram baixados após o npm install.

public: onde de forma pública se armazena as imagens e fontes.

src: onde foi posto os códigos.
Dentro da src tem os:

   assets: é onde de forma privada consegue guardar imagens e fontes.

   components: são funções que tornam o desenvolvimento mais organizado e eficiente, por serem códigos isolados fica melhor ao fazer alterações por não afetar o restante.
   Dentro de components tem o BannerAd.jsx colocado para caso de propaganda e a NavBar.jsx a barra superior.
   Os dois se encontram em todas as pages sem ter sido reescritos.

   pages: onde foi posto as paginas DpoLgpd, Noticias, Faculdade, Inicial e Visualizar Noticias. Todas routeadas no App.jsx e linkadas na barra superior (NavBar).
   
   admin: onde foi posta as funcionalidades dos admins, podendo alterar as noticias.

   A seguir são dois arquivos que estão fora dos packages da src:
   
   App.jsx: ele é o arquivo pai onde os componentes são chamados e faz o roteamento para todas as páginas

   App.css e Main.css: servem para estilizar o projeto, porém não foram usados, pois as bibliotecas Mui e Emotion foram as escolhidas para esse papel de estilização.

Fora dos packages tem os arquivos:
	
   .gitignore: existe para o git saber quais files ou packages ignorar ao fazer o versionamento do código.
	
   eslint.config.js: onde está algumas das configurações do projeto.

   index.html: onde foram chamados os scripts.

   package-lock.json e package.json: onde está as dependências e bibliotecas que foram instaladas, além de algumas configurações do node.
   
   README.md: utilizado para por informações sobre o projeto.
	
   vite.config.js: onde fica as configurações do VITE.



Bibliotecas usadas:

  React Router Dom: Biblioteca utilizada para criar rotas, ela mapeia as URLs para os componentes sem precisar que a página seja recarregada.
	npm install react-router-dom

  Json server: Simula um back-end sem ter um banco de dados real. Simula uma api restful.
  	npm install json-server

    Mui e Emotion: São bibliotecas usadas para estilizar.
	npm install @mui/material @emotion/react @emotion/styled
	npm install @mui/icons-material --legacy-peer-deps

  Axios: Biblioteca que é utilizada para fazer requisições HTTP, ela faz o envio ou o recebimento de dados de forma assíncrona.
	npm install axios
