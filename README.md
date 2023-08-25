# VueJS_Project01


## Desenvolvimento



### Visual Studio Code

_Extensões recomendadas:_

-   Vetur
-   ESLint
-   Prettier - Code formatter
-   Sass
-   ENV

_Configurações recomendadas:_

-   Formatter do Vetur: Prettier (exceto para Sass)
-   Ativar Format on save
-   Ativar Trim trailing whitespace




### Comandos para criação de um projeto VueJS + VueCLI

Instalar o ambiente
	NVM --> Node Version Manager
		Link para instalação
			https://github.com/nvm-sh/nvm
		Descrição
			navega entre as versões do NPM
			gerenciador de versão do node
			ferramenta de desenvolvimento instalação do Node e outras específicas
			instalando pelo "apt" da muito problema por conta do gerenciamento de pastas 
				problema na permissã pq foi instalado pelo gerenciador de pacote
	Ferramentas de desenvolvimento NODE
		Descrição:
			Gerencidor de pacotes
			faz uma bild do código para colocar no ar
				de desenvolvimento e produção (minificação)
		YARN
			npm install -g yarn
				instalando o YARN via NPM
			yarn --version
			na pasta do projeto
			yarn create nuxt-app ["nome_do_projeto"] --> criar o projeto naxt 
				Ex.: yarn create nuxt-app vueproject
		NPM
			npm -version
			npm -versionigual ao YARN
			o NPM tem de ser instaldo pelo NVM
			O YARN é instala o NPN
	Node.js 
		sudo apt-get install -y nodejs
		node -v
	VueCLI
		npm install -g @vue/cli
			sudo npm install -g vue-cli@2.7.0
		yarn global add @vue/cli
		vue --version
	VSCode
		Extensõe vue do Liuji-jim
criar projeto novo do zero
	*instalar o VueCLI
	vue create ["nome_do_projeto"]
		escolher a versão [Vue 3]
criar projeto novo a partir de um template
	navegar até a pasta de destino
		vue init webpack-simple [nome_do_projeto]
			precionar ENTER	em todas as opções
	navegar ate a pasta do projeto criado
			npm install
				baixa todas as dempedencias
			npm run dev
				executa o projeto criado
				URL de acesso: http://localhost:3000/pt-br
Instalando outros pacotes
	Vuex ?? perguntar para o Caio
		??? npm install --save vuex@next
		ou
		??? yarn add vuex
Rodando subindo o proljeto
	YARN
		yarn install
		yarn server
	NPM 
		*dentro da pasta do APP
		npm install
		npm run dev
		Utilizando ultima versão estavel --> trocar verção do node v17 para node 16.14.0
			nvm list 
			node -v
			nvm use --l