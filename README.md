# Code Challenge

Primeiramente, vale-se notar que esse desafio consiste de duas partes, frontend e backend. Caso o candidato esteja almejando uma posição frontend, apenas essa parte deve ser realizada. Caso esteja almejando uma backend, apenas essa deve ser feita. Por fim, caso esteja almejando uma posição full stack, ambos devem ser realizados, frontend e backend, com as respectivas integrações. De forma superficial, a tarefa, frontend, consiste em clonar as páginas "Início", "Dados Básicos" e "Localização" de preparovc.com/perfil, em ReactJS; Quanto ao backend, deve desenvolver um capaz de intermediar as requisições entre frontend e MongoDB, sendo feito em NodeJS; No processo full stack, além dos descritos de frontend e backend, o candidato também deve realizar um projeto que intregre o frontend com o Firebase. 

## Frontend
    
A parte de frontend consiste em clonar as seguintes páginas utilizando-se de ReactJS:
-   [Início](https://preparovc.com/perfil);
-   [Dados básicos](https://preparovc.com/perfil/formsperfil);
-   [Localização](https://preparovc.com/perfil/formslocalizacao).

### O que será avaliado
    - Componentização;
    - Responsividade;
    - Verificação de dados (via Regex) e menssagens de erro;
    - Construção do style (CSS, por exemplo);
    - Limpeza e organização do código;
    - Navegação (Facilidade para transitar entre páginas);
    - Utilização do Javascript/Typescript.

### Observação
A similaridade de ícones será desconsiderada na correção. 


## Backend

O Candidato deve conceber um projeto que integre um frontend fictício. O Projeto deve:
-   Ser capaz de cadastrar um usuário
-   Ser capaz de autenticar um usuário
-   Armazenar, editar e excluir as informações fornecidas pela página [Dados básicos](https://preparovc.com/perfil/formsperfil);
-   Armazenar, editar e excluir as informações fornecidas pela página [Localização](https://preparovc.com/perfil/formslocalizacao);

### Algumas considerações sobre a conexão com os bancos de dados
    - Fica a critério do candidato escolher como organizar a estrutura do banco de dados ( _MongoDB_);
    - É esperado que o banco de dados inicie vazio;
    - O candidato pode optar por utilizar _MongoDB_ localmente ou utilizar a hospedagem _MongoDB Atlas_;
    - Se o banco de dados _MongoDB_ for hospedado no _MongoDB Atlas_, a equipe da Preparo deve ter acesso para leitura e escrita (ver Acesso ao projetos);

### O que será avaliado
    - Clareza do código;
    - Boas práticas de programação (indentação, acoplamento, nomes de variáveis etc.);
    - Bom senso ao seguir instruções;
    - Estrutura do banco;


## Full stack

O Candidato deve realizar tanto a parte de frontend quanto backend. Além disso, deve ser realizado um projeto, o qual utiliza-se do firebase.Deve ser feito, além do descrito nas partes anteriores:
-   A crição das páginas de  _login_ e cadastro, as quais os _layouts_ não precisam ser fiéis ao original;
-   Se o candidato preferir, pode ser feito um projeto _frontend_ para a versão _Firestore/Storage_ e outro para a versão _MongoDB/Storage_, mas ambos precisam ser indistintos visualmente ao serem acessados pelo navegador (sem inspecionar o código, o usuário não deve ser capaz de saber qual banco de dados está sendo utilizado);
-   O projeto frontend **pode** acessar _Firebase Auth_ diretamente (sem necessidade de um _backend_) sem quaisquer penalidades diretas;
-   O projeto frontend **pode** enviar e receber dados do _Firebase Firestore_ e _Firebase Storage_ diretamente (mas pode ser intermediado por um _backend_ se o candidato assim preferir);

### Cadastro
    - O usuário deve ser capaz de criar uma conta (utilizando Firebase Auth, no projeto Firebase e via backend, no projeto MongoDB);
    - Caso o usuário já possua uma conta, ele pode facilmente navegar para a página de login;

### Login
    - O usuário deve ser capaz de fazer login na plataforma utilizando sua conta criada anteriormente (utilizando Firebase Auth, no projeto Firebase e via backend, no projeto MongoDB);
    - O usuário deve ser capaz de facilmente navegar para a página de cadastro caso ainda não possua uma conta;

## Dados Básicos
    - O usuário precisa ser capaz de salvar/atualizar suas informações (inclusive email e foto de perfil) (utilizando Firebase firestore/storage, no projeto Firebase e via backend, no projeto MongoDB);

### Localização
    - O usuário precisa ser capaz de atualizar suas informações de localização (utilizando Firebase firestore/storage, no projeto Firebase e via backend, no projeto MongoDB);

### Algumas considerações sobre a conexão com os bancos de dados
    - Fica a critério do candidato escolher como organizar a estrutura do banco de dados (_Firestore_);
    - É esperado que o banco de dados inicie vazio;
    - A equipe da Preparo deve ter acesso ao projeto do _Firebase_ (ver Acesso ao projetos);

### O que será avaliado
    - Os itend das partes frontend e backend;
    

## Acesso aos projetos

Para dar acesso aos projetos, convide `tech@preparovc.com` para participar do projeto privado no Github, Firebase e MongoDB Atlas (se necessário). Para o Firebase, permisão de _editor_ é suficiente. Por fim, além de dar acesso aos projetos, preencha [este formulário](https://forms.gle/eWSU5cArcMyNodiy9).

# FAQ

**1. É necessário armazenar imagens no Firebase Storage ou pode ser armazenado localmente?**<br>
É necessário usar o Firebase Storage para armazenar imagens.

**2. É necessário esconder as variáveis de ambiente no `.gitignore`?**<br>
Por questões de simplificação, não é necessário esconder as variáveis de ambiente no `.gitignore`.

**3. Pode usar pacotes como `express` para o desenvolvimento do _backend_?**<br>
Sim, é permitido usar pacotes como `express`, `mongoose`, `morgan` e/ou outros que o candidato achar necessário para o desenvolvimento do _backend_.

**4. Estou fazendo o processo de _frontend_, devo fazer todo o challenge?**<br>
Não! Caso esteja realizando o processo de frontend, apenas essa parte deve ser realizada.

**5. O projeto frontend pode enviar ou receber dados do _MongoDB_ diretamente?**<br>
O projeto frontend **não pode** enviar ou receber dados do _MongoDB_ diretamente (é necessária a construção de um _backend_ para isso);
