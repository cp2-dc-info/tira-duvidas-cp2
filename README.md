# tira-duvidas-cp2
Tira duvidas cp2

## Requisitos Funcionais

### RF01

O sistema deverá armazenar usuários com login, nome, email, senha e imagem de perfil.

### RF02

O sistema deverá armazenar perguntas, que contém um título e um autor

### RF03

O sistema deverá armazenar respostas, que possuem autor, data e hora, conteúdo, a pergunta à qual pertence e a quantidade de votos positivos.

### RF04

O sistema deverá pesquisar perguntas

## Casos de Uso

### CDU01 - Cadastro
  - Pré-requisitos: nenhum
  - Fluxo principal
    + O usuário preenche o formulário de cadastro e clica no botão cadastrar
    + O Sistema valida as informações, salva o usuário e redireciona para a tela de login
  - Fluxo alternativo
    + O usuário preenche o formulário de cadastro e clica no botão cadastrar
    + O sistema informa os erros de preenchimento do formulário
    + O usuário corrige os erros e envia novamente o formulário
    + O Sistema valida as informações, salva o usuário e redireciona para a tela de login

### CDU02 - Login
  - Pré-requisitos: o usuário precisa estar cadastrado no sistema
  - Fluxo principal
    + O usuário preenche o email e senha e clica no botão login
    + O Sistema verifica a senha do usuário e , salva o usuário e redireciona para a tela de login
  - Fluxo alternativo
    + O usuário preenche o email e senha e clica no botão login
    + O sistema informa que o email e senha não coincidem
    + O usuário corrige suas informações de login e envia novamente o formulário
    + O Sistema valida as informações e redireciona o usuário para o Feed

### CDU02 - Perguntar
  - Pré-requisitos: o usuário precisa estar autenticado no sistema
  - Fluxo principal
    + O usuário escreve uma pergunta e clica no botão perguntar
    + O Sistema verifica se o formulário não está vazio e salva a pergunta
  - Fluxo alternativo
    + O usuário escreve uma pergunta e clica no botão perguntar
    + O Sistema informa que o formulário está vazio
    + O usuário corrige sua pergunta e envia novamente
    + O Sistema verifica se o formulário não está vazio e salva a pergunta

### CDU02 - Responder
  - Pré-requisitos: o usuário precisa estar autenticado no sistema
  - Fluxo principal
    + O usuário seleciona uma pergunta, escreve uma resposta e clica no botão responder
    + O Sistema verifica se o formulário não está vazio e salva a resposta
  - Fluxo alternativo
    + O usuário seleciona uma pergunta, escreve uma resposta e clica no botão responder
    + O Sistema informa que o formulário está vazio
    + O usuário corrige sua resposta e envia novamente
    + O Sistema verifica se o formulário não está vazio e salva a resposta

### CDU02 - Votar
  - Pré-requisitos: o usuário precisa estar autenticado no sistema
  - Fluxo principal
    + O usuário seleciona uma pergunta, clica no botão "Entendi!" em uma resposta
    + O Sistema soma 1 na quantidade de votos da resposta
  - Fluxo alternativo
    + O usuário seleciona uma pergunta, clica no botão "Entendi!" em uma resposta
    + O Sistema informa que o usuário já votou naquela resposta
    
### CDU02 - Pesquisar
  - Pré-requisitos: nenhum
  - Fluxo principal
    + O usuário preenche a barra de pesquisa e clica em pesquisar
    + O Sistema mostra todas as perguntas que possuem o texto buscado
  - Fluxo alternativo
    + O usuário preenche a barra de pesquisa e clica em pesquisar
    + O Sistema informa que nao perguntar que coincidem com a busca
    
### CDU02 - Feed
  - Pré-requisitos: nenhum
  - Fluxo principal
    + O sistema apresenta a lista de perguntas ordenada da mais recente para a mais antiga
    + O usuário clica em uma pergunta e o sistema dereciona para uma tela que exibe as respostas
    
    
