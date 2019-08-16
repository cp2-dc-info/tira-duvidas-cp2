# tira-duvidas-cp2
Tira duvidas cp2

## Requisitos Funcionais

### RF01

O sistema deverá armazenar usuários com login, nome, email, senha e imagem de perfil.

### RF02

O sistema deverá armazenar perguntas, que contém um título e um autor

### RF03

O sistema deverá armazenar respostas, que possuem autor, data e hora, conteúdo, a pergunta à qual pertence e a quantidade de votos positivos.

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

