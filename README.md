# ByteBank Vuex

Neste projeto utilizei Vue 2 para explorar como funciona o Vuex.

A idéia do projeto é permitir que seja realizado um cadastro de usuário básico, com login e senha. Após isso, é realizada a autenticação e armazenado o token do usuário, permitindo que sejam realizadas outras operações.

Como exemplo, após a realização do login, o usuário poderá realizar listagem de recursos através de um endpoint que requer autenticação.

Neste projeto foi utilizado o Vuex para armazenamento do usuário no estado global, para que qualquer componente possa ter acesso ao objeto do usuário de forma simples e direta, respeitando o padrão do Vuex, com Actions e Mutations.

## Como rodar no localhost

###  Clonar o repositório

```sh
git clone git@github.com:AmandaSoaress/bytebank-vuex.git
```

Por ser tratar do framework Vue, é necessário a instalação de todas as dependências que o projeto funcione corretamente. Para isso, é necessário ter o `node` e  o `npm` instalados na maquina.

Eu utilizei o `node` na versão `v12.22.12` e o `npm` na versão `6.14.16`.

###  Instalar dependências

Abra a pasta do projeto e execute o `npm install`:

```sh
cd bytebank-vuex
npm install
```

### Iniciar o projeto

Após a instalação dos pacotes, basta iniciar o projeto:

```sh
npm run serve
```

Pronto, você já está rodando o projeto em seu computador.

## Build para Deploy

Para fazer a build e obter os arquivos estáticos, você pode executar:

```sh
npm run build
```


!["Página de login"](img\preview-login.png)
<br><br>
!["Lista de Gerentes"](img\preview-gerentes.png)