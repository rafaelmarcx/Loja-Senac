

# Simulação de E-commerce - Projeto Next.js

## Visão Geral - Fase 1

Este projeto é uma simulação de uma plataforma de e-commerce desenvolvida pelos alunos. O foco inicial será na construção da interface do usuário, seguida pelo desenvolvimento do back-end e da camada de dados. O projeto utiliza Next.js como framework e MUI (Material-UI) para os componentes da interface.

O projeto será dividido em diferentes funcionalidades, atribuídas a grupos de estudantes (duplas ou um trio). Cada grupo será responsável por desenvolver uma parte específica da interface front-end. Após completar a interface, avançaremos para as outras camadas da aplicação.

LINK DE EXEMPLO: https://bazaar.ui-lib.com/market-2


## Funcionalidades Atribuídas

Cada dupla/trio será responsável pela implementação de uma funcionalidade específica da interface. Abaixo estão as atribuições de funcionalidades:

- Yan & Vitor Hugo: Página de Login
- Welker & Tais: Componente de Card de Produto
- Vitor & Richard: Página de Listagem de Produtos
- Lorran & Davi Vale: Barra de Navegação
- Daniel & Erica: Página de Checkout
- Raphael & Davi: Página de Detalhes do Produto
- Augusto, Arthur & Pedro: Carrinho de Compras

## Estrutura do Projeto

O projeto é construído com Next.js e utiliza MUI para estilização e layout dos componentes. Os alunos focarão nos seguintes pontos:

- Criar componentes reutilizáveis para a interface.
- Cada funcionalidade terá sua própria branch de desenvolvimento.
- Testar componentes em páginas dedicadas antes de integrá-los ao projeto.

# Fase 2: Desenvolvimento do Back-end e Integração de Dados

## Objetivos:

- Desenvolver as APIs necessárias para o e-commerce.
- Conectar a interface desenvolvida na Fase 1 com o back-end.
- Criar e configurar a base de dados usando MongoDB Atlas para armazenar informações sobre produtos, usuários, pedidos e carrinho de compras.
- Implementar autenticação e autorização de usuários usando NextAuth.js.
- Garantir que a aplicação seja funcional e escalável.

# Stack Tecnológico 

- Next.js (Framework React)
- MUI (Material-UI) (Biblioteca de componentes de interface)
- Node.js com Express para o desenvolvimento do back-end.
- MongoDB Atlas para armazenamento de dados.
- NextAuth.js para autenticação e autorização.
- Axios ou Fetch API para consumo das APIs no front-end.

## Tarefas por Grupos:

1. Yan & Vitor Hugo - Autenticação de Usuário com NextAuth.js
- Descrição: Implementar a autenticação de usuários usando NextAuth.js para simplificar o processo de login e registro.
### Tarefas:
- Configurar o NextAuth.js no projeto, utilizando provedores de autenticação (Google, GitHub ou credenciais).
- Conectar o NextAuth com o MongoDB Atlas para armazenar e gerenciar os dados dos usuários.
- Adicionar proteção de páginas no front-end, restringindo o acesso a determinadas áreas somente para usuários autenticados.

2. Welker & Tais - API de Produtos
- Descrição: Desenvolver a API responsável por manipular os dados dos produtos.
### Tarefas:
- Criar rotas para GET, POST, PUT e DELETE de produtos.
- Utilizar o MongoDB Atlas para armazenar, buscar e alterar os dados dos produtos.
- Testar o componente de card de produto integrado com a API, exibindo dados reais na interface.

3. Vitor & Richard - Listagem e Filtros de Produtos
- Descrição: Implementar o sistema de listagem e filtragem dos produtos, consumindo a API desenvolvida.
### Tarefas:
- Consumir a API de produtos e renderizar a listagem na página de produtos.
- Implementar filtros por categoria, preço e avaliação dos produtos.
- Conectar a interface de filtro com a API para obter os dados filtrados em tempo real.

4. Lorran & Davi Vale - Navegação e Rotas Protegidas
- Descrição: Melhorar a navegação da aplicação e implementar rotas protegidas com NextAuth.js, acessíveis apenas para usuários autenticados.
### Tarefas:
- Configurar o sistema de rotas protegidas usando o NextAuth.js.
- Proteger rotas como o Carrinho e Checkout, redirecionando usuários não autenticados para a página de login.
- Testar a navegação integrada com o estado de autenticação dos usuários.

5. Daniel & Erica - API de Checkout e Pedidos
- Descrição: Desenvolver a API responsável pelo processo de checkout e criação de pedidos.
### Tarefas:
- Criar rotas de checkout e pedidos (POST para criar pedidos, GET para visualizar pedidos do usuário).
- Utilizar o MongoDB Atlas para armazenar as informações dos pedidos (produtos, preços e status).
- Integrar a página de checkout com a API.

6. Raphael & Davi - Página de Detalhes do Produto e Avaliações
- Descrição: Implementar a funcionalidade de avaliações dos produtos e integrar a API com a página de detalhes do produto.
### Tarefas:
- Criar a funcionalidade para que os usuários possam visualizar e adicionar avaliações nos produtos.
- Utilizar o MongoDB Atlas para armazenar e buscar as avaliações.
- Integrar a API de produtos para exibir dados reais dos produtos na página de detalhes.

7. Augusto, Arthur & Pedro - API do Carrinho de Compras
- Descrição: Desenvolver a API e a interface do carrinho de compras.
### Tarefas:
- Criar rotas para manipulação do carrinho de compras (ADD, UPDATE e REMOVE itens).
- Utilizar o MongoDB Atlas para armazenar e gerenciar os itens do carrinho por usuário.
- Testar a integração entre a API e o front-end, exibindo os itens do carrinho de cada usuário autenticado.

# Como utilizar MONGODB ATLAS
- Instale mongodb no projeto
```
npm install mongodb
```

- URL do Banco de Dados: "mongodb+srv://vinicioscararine95:Navaronee897157@cluster0.3pfo9yd.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0"


## Branches e Pull Requests

Cada grupo trabalhará em sua funcionalidade em uma branch separada. Os nomes das branches devem corresponder à funcionalidade que estão desenvolvendo. Por exemplo:

- Yan & Vitor Hugo trabalharão na página de login na branch /login.
- Welker & Tais trabalharão no card de produto na branch /product-card.

# Fluxo de Trabalho:

1. Fork do Repositório: Cada aluno deve fazer o fork do repositório principal para sua própria conta no GitHub..

2. Criar uma Branch para Sua Funcionalidade: Após o fork, crie uma branch que corresponda à funcionalidade que está desenvolvendo (por exemplo, /login, /product-card).

3. Atualize Seu Fork: Antes de começar qualquer desenvolvimento, sempre garanta que seu fork esteja atualizado com as últimas mudanças da branch master:

```
git fetch origin
git pull origin master
```

4. Desenvolva e Teste:

- Enquanto desenvolve um componente, crie uma página de teste para garantir que tudo funcione como esperado. Esta página é apenas para testes internos e não deve ser incluída na PR final.
- Por exemplo, se você está trabalhando no card de produto, crie uma página onde você possa ver o componente renderizado na tela e testar seu comportamento.

5. Submeta Apenas o Componente: Uma vez que sua funcionalidade esteja pronta, não envie a página de teste. Envie apenas a pasta e o(s) arquivo(s) respectivo(s) à sua funcionalidade (por exemplo, components/Card.js).

6. Abra uma Pull Request: Quando estiver pronto, submeta sua funcionalidade por meio de uma pull request para a branch correspondente:

- Yan & Vitor Hugo enviarão uma PR para /login.
- Welker & Tais enviarão uma PR para /product-card.
- E assim por diante.

## Boas Práticas

- Sempre Atualize Seu Repositório: Antes de iniciar qualquer novo trabalho, sempre atualize seu repositório para a versão mais recente:

```
git fetch origin
git pull origin master

```

- Commits Pequenos: Faça commits incrementais e frequentes. Isso ajuda a evitar commits grandes e difíceis de gerenciar.

- Rebase com Master: Após o merge de uma pull request de outro grupo, garanta que você faça o rebase da sua branch com a versão mais recente da master:

```
git fetch origin
git rebase origin/master

```

- Isso evita conflitos antes de enviar sua pull request.

- Commits Claros e Objetivos: Use mensagens de commit descritivas, como "Adicionada validação do formulário de login" ou "Criado componente reutilizável de card de produto".


## Conclusão

Este projeto simula um cenário de desenvolvimento real, onde cada grupo contribui independentemente para construir uma aplicação coesa. Certifique-se de colaborar, seguir sua funcionalidade atribuída e respeitar o fluxo de trabalho para garantir uma integração suave entre todas as funcionalidades.

Boa sorte e vamos construir algo incrível juntos!
