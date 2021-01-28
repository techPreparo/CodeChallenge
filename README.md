# Code Challenge

A tarefa consiste em clonar o frontend (ReactJS) "Dados Básicos" e "Localização" de preparovc.com/perfil; O candidato deve desenvolver um backend (NodeJS) capaz de intermediar as requisições entre frontend e MongoDB;

## Páginas a serem clonadas

-   _login_/cadastro (não precisa ser visualmente fiel ao _login_/cadastro da Preparo);
-   [Início](https://preparovc.com/perfil) (no caso de haver instruções específicas que o candidato considere importantes);
-   [Dados básicos](https://preparovc.com/perfil/formsperfil);
-   [Localização](https://preparovc.com/perfil/formslocalizacao);

## O que é esperado

-   Pelo menos 1 projeto _frontend_ utilizando _ReactJS_ com as páginas a serem clonadas;
-   O _layout_ das páginas de _login_ e cadastro não precisam ser fiéis ao original;
-   O _layout_ das páginas de perfil precisam ser fiéis ao original (considerando cores, posição dos elementos, imagens, funcionalidades e desconsiderando ícones e tipografia);
-   O projeto frontend **pode** acessar _Firebase Auth_ diretamente (sem necessidade de um _backend_) sem quaisquer penalidades diretas;
-   O projeto frontend **pode** enviar e receber dados do _Firebase Firestore_ e _Firebase Storage_ diretamente (mas pode ser intermediado por um _backend_ se o candidato assim preferir);
-   O projeto frontend **não pode** enviar ou receber dados do _MongoDB_ diretamente (é necessária a construção de um _backend_ para isso);
-   Se o candidato preferir, pode ser feito um projeto _frontend_ para a versão _Firestore/Storage_ e outro para a versão _MongoDB/Storage_, mas ambos precisam ser indistintos visualmente ao serem acessados pelo navegador (sem inspecionar o código, o usuário não deve ser capaz de saber qual banco de dados está sendo utilizado);
-   Pelo menos 1 projeto _backend_ para intermediar o frontend e o MongoDB;

## O que será avaliado

    - Clareza do código;
    - Boas práticas de programação (indentação, acoplamento, nomes de variáveis etc.);
    - Bom senso ao seguir instruções;

## Cadastro

-   O usuário deve ser capaz de criar uma conta (utilizando Firebase Auth);
-   Caso o usuário já possua uma conta, ele pode facilmente navegar para a página de login;

## Login

-   O usuário deve ser capaz de fazer login na plataforma utilizando sua conta criada anteriormente;
-   O usuário deve ser capaz de facilmente navegar para a página de cadastro caso ainda não possua uma conta;


## Dados Básicos

-   O usuário precisa ser capaz de salvar/atualizar suas informações (inclusive email e foto de perfil);
-   O _layout_ da página deve ser fiel, na medida do possível, ao da página original. A tipografia e os ícones podem ser arbitrários desde que sejam adequados ao contexto;


## Localização

-   O usuário precisa ser capaz de atualizar suas informações de localização;


## Algumas considerações sobre a conexão com os bancos de dados

-   Fica a critério do candidato escolher como organizar a estrutura do banco de dados (_Firestore_ e _MongoDB_);
-   É esperado que o banco de dados inicie vazio;
-   O candidato pode optar por utilizar _MongoDB_ localmente ou utilizar a hospedagem _MongoDB Atlas_;
-   Se o banco de dados _MongoDB_ for hospedado no _MongoDB Atlas_, a equipe da Preparo deve ter acesso para leitura e escrita;
-   A equipe da Preparo deve ter acesso ao projeto do _Firebase_;


## Acesso aos projetos

Para dar acesso aos projetos, convide `tech@preparovc.com` para participar do projeto privado no Github, Firebase e MongoDB Atlas (se necessário). Para o Firebase, permisão de _editor_ é suficiente.

# FAQ

**1. É necessário armazenar imagens no Firebase Storage ou pode ser armazenado localmente?**<br>
É necessário usar o Firebase Storage para armazenar imagens.

**2. É necessário esconder as variáveis de ambiente no `.gitignore`?**<br>
Por questões de simplificação, não é necessário esconder as variáveis de ambiente no `.gitignore`.

**3. Pode usar pacotes como `express` para o desenvolvimento do _backend_?**<br>
Sim, é permitido usar pacotes como `express`, `mongoose`, `morgan` e/ou outros que o candidato achar necessário para o desenvolvimento do _backend_.
