# Criar casos de testes para o fluxo de cadastro da pessoa usuária

1. **Cenário geral do login da Plataforma Coursera.org**

A plataforma Coursera oferece cursos em diversas áreas do mercado. Ela oferece quatro formas de permissão de acesso -  Individual, Negócios, Universitarios e Gorvernamental, nesta plataforma o interessado deve fazer registro na página inicial (https://www.coursera.org/) para então se inscrever em um curso que pode ser gratuito ou pago. Dentro das suas funcionalidades iniciais estão, busca de cursos (sem estar registrado na plataforma), cadrastro de usuário, caixa de login, clicando em um curso o usuário tem acesso as informações resumidas sobre o curso, avaliação do curso por outros usuários, data de inclusão do curso na plataforma, instrutor/professor do curso, idioma que ele foi desenvolvido e quanto tempo o usuário irá realiza-lo além de se for pago o valor de aquisição.

Regra de negócios tem como requisitos o cadastro de uma nova pessoa usuária a partir dos seguintes dados fornecidos:

- Nome que deve conter apenas letras;
- Sobrenome que deve conter apenas letras;
- E-mail válido e ativo;
- Senha que contenha no mínimo 8 caracteres dentre eles letra maiúscula, letra minúscula, número, caractere especial (ex: #!*-_&) e as senhas devem ser iguais na caixa de checagem;
- O fluxo de cadastro da pessoa usuária deve permitir que uma nova pessoa usuária se registre no sistema;

# **Cenários de teste**

## **Cenário 1:**

Pessoa usuária fornece informações válidas.

**Entrada:**

- Nome: Elisete
- Sobrenome: Cercal
- E-mail: elisetedscercal@icloud.com
- Senha: Elisete@123

**Saída:**

**Pessoa usuária é registrado com sucesso.**

| Caso de Teste Cadastro de pessoa usuária | Passos | Resultado esperado | Resultado Teste 1 |
| --- | --- | --- | --- |
| CT1: Usuário fornece informações válidas. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | É exibida a página “Bem vinda à Lacrei” com o campo  de “Login” . | Página home será exibida “Bem vinda à Lacrei” |
|  | Clicar no botão “Criar  conta” | Formulário de cadastro será exibido | Formulário de cadastro foi exibido |
|  | Preencher os campos obrigatórios com informações válidas | Os campos devem receber dados digitados | Todos os campos foram preenchidos com dados digitáveis e já cadastrados. |
|  | Marcar o campo de "Li e concordo com termos de uso” | O campo deve ficar marcado de branco para verde | O campo ficou marcado de branco para verde |
|  | Marcar o campo de “tenho mais de 18 anos” | O campo deve ficar marcado de branco para verde | O campo deve ficou marcado de branco para verde |
|  | Clicar no botão “cadastrar” | O sistema apresenta uma mensagem para confirmação de e-mail “Para sua segurança,
enviamos um link de verificação para o e-mail cadastrado” | O sistema apresentou uma mensagem para confirmação de e-mail “Para sua segurança,
enviamos um link de verificação para o e-mail cadastrado” |
|  | Após o recebimento do link de verificação na caixa de e-mail da nova pessoa cadastrada, clicar no link para confirmar e-mail | O sistema apresenta uma menssagem para confirmação de e-mail “Para sua segurança,
enviamos um link de verificação para o e-mail cadastrado” | O sistema apresentou uma menssagem para confirmação de e-mail “Para sua segurança,
enviamos um link de verificação para o e-mail cadastrado” |

**Teste 1**

![CT1.gif](Criar%20casos%20de%20testes%20para%20o%20fluxo%20de%20cadastro%20da%20/CT1.gif)

## **Cenário 2:**

Pessoa usuária fornece informações inválidas.

**Entrada:**

- Nome: n/a
- Sobrenome: Cercal
- E-mail: elisetecercal@gmail.com
- Senha: n/a
- Senha repetição de senha para confirmação: n/a

**Saída:**

**Pessoa usuária não é registrado.**

| Caso de Teste Cadastro de pessoa usuária | Passos | Resultado esperado | Resultado Teste |
| --- | --- | --- | --- |
| CT2: Usuário fornece informações válidas e campos vazios (inválidas). | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | É exibida a página “Bem vinda à Lacrei” com o campo  de “Login” . | Página home será exibida “Bem vinda à Lacrei” |
|  | Clicar no botão “Criar  conta” | Formulário de cadastro será exibido | Formulário de cadastro foi exibido |
|  | Preencher alguns dos campos obrigatórios com informações válidas e outros deixar vazio. | Os campos “nome”e “senha” não devem receber dados digitados ou seja vazios. Apenas os campos “e-mail”e "sobrenome". | Os campos “nome”e “senha” não receberam  dados digitados ou seja vazios. Apenas os campos “e-mail”e "sobrenome". |
|  | Marcar o campo de "Li e concordo com termos de uso” | O campo deve ficar marcado de branco para verde | O campo  ficou marcado de branco para verde |
|  | Marcar o campo de “tenho mais de 18 anos” | O campo deve ficar marcado de branco para verde | O campo deve ficou marcado de branco para verde |
|  | Clicar no botão “cadastrar” | O sistema apresenta as mensagens “o nome é obrigatório”, “a senha é obrigatória” e “a confirmação de senha é obrigatória”. Não realizando o cadastro da nova pessoa usuária. | O sistema apresentou as mensagens “o nome é obrigatório”, “a senha é obrigatória” e “a confirmação de senha é obrigatória”. Não realizou o cadastro da nova pessoa usuária como esperado. |

**Teste 2**

![CT2.gif](Criar%20casos%20de%20testes%20para%20o%20fluxo%20de%20cadastro%20da%20/CT2.gif)

---

---

## **Cenário 3:**

Pessoa usuária já está cadastrado.

**Entrada:**

- Nome: Elisete
- Sobrenome: Cercal
- E-mail: elisetecercal@gmail.com
- Senha: Elisete@123
- Senha repetição de senha para confirmação: @123

**Saída:**

**Pessoa usuária não é registrado.**

| Caso de Teste Cadastro de pessoa usuária | Passos | Resultado esperado | Resultado Teste |
| --- | --- | --- | --- |
| CT3: pessoa usuária fornece informações válidas já cadastradas no sistema. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | É exibida a página “Bem vinda à Lacrei” com o campo  de “Login” . | Página “Bem vinda à Lacrei” foi exibida com o campo “Login” |
|  | Clicar no botão “Criar  conta” | É exibido o formulário de cadastro será exibido | Formulário de cadastro foi exibido |
|  | Preencher os campos obrigatórios com informações válidas |  Todos os campos devem ser preenchidos com dados digitáveis e já cadastrados. | Todos os campos foram preenchidos com dados digitáveis e já cadastrados. |
|  | Marcar o campo de "Li e concordo com termos de uso” | O campo deve ficar marcado de branco para verde | O campo ficou marcado de branco para verde |
|  | Marcar o campo de “tenho mais de 18 anos” | O campo deve ficar marcado de branco para verde | O campo ficou marcado de branco para verde |
|  | Clicar no botão “cadastrar” | O sistema deve apresenta uma mensagem “Um usuário já foi registrado com este endereço de e-mail.” não realizando o cadastro. | O sistema apresenta uma mensagem “Um usuário já foi registrado com este endereço de e-mail.” não realizou o cadastro conforme esperado. |

**Teste 3**

![CT3.gif](Criar%20casos%20de%20testes%20para%20o%20fluxo%20de%20cadastro%20da%20/CT3.gif)

---

---

## **Cenário 4:**

Pessoa usuária não cadastrada fornece senha com somente números.

**Entrada:**

- Nome: Elisete
- Sobrenome: Cercal
- E-mail: elisetecercal@gmail.com
- Senha: 123455678

**Saída:**

**Pessoa usuária não é registrado.**

| Caso de Teste Cadastro de pessoa usuária | Passos | Resultado esperado | Resultado esperado |
| --- | --- | --- | --- |
| CT4: Usuário fornece informações válidas mas com campo senha apenas números. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | É exibida a página “Bem vinda à Lacrei” com o campo  de “Login” . | Página “Bem vinda à Lacrei” foi exibida com o campo “Login” |
|  | Clicar no botão “Criar  conta” | Formulário de cadastro será exibido | Formulário de cadastro foi exibido |
|  | Preencher os campos obrigatórios com informações válidas |  Todos os campos são preenchidos com dados digitáveis, onde campo "senha”recebe apenas números |  Todos os campos foram preenchidos com dados digitáveis, onde campo "senha”recebe apenas números |
|  | Marcar o campo de "Li e concordo com termos de uso” | O campo deve ficar marcado de branco para verde | O campo  ficou marcado de branco para verde |
|  | Marcar o campo de “tenho mais de 18 anos” | O campo deve ficar marcado de branco para verde | O campo  ficou marcado de branco para verde |
|  | Clicar no botão “cadastrar” | O sistema apresenta o campo “senha” em vermelho e sinaliza também em vermelho os dados obrigatórios para o campo “senha”, neste caso letras maiúsculas, letras minúsculas e caracteres especiais. Pessoa usuária não é registrada. | O sistema apresentou o campo “senha” em vermelho e sinaliza também em vermelho os dados obrigatórios para o campo “senha”, neste caso letras maiúsculas, letras minúsculas e caracteres especiais. Pessoa usuária não é registrada. |

**Teste 4**

![CT4.gif](Criar%20casos%20de%20testes%20para%20o%20fluxo%20de%20cadastro%20da%20/CT4.gif)

## **Cenário 5:**

Pessoa usuária não cadastrada fornece senha com somente letras minúsculas

**Entrada:**

- Nome: Elisete
- Sobrenome: Cercal
- E-mail: elisetecercal@gmail.com
- Senha: elisetecercal

**Saída:**

**Pessoa usuária não é registrado.**

| Caso de Teste Cadastro de pessoa usuária | Passos | Resultado esperado | Resultado Teste |
| --- | --- | --- | --- |
| CT5: Usuário fornece informações válidas mas com campo “senha” apenas letras minúsculas. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | Página “Bem vinda à Lacrei” foi exibida com o campo “Login” | Página home será exibida “Bem vinda à Lacrei” |
|  | Clicar no botão “Criar  conta” | Formulário de cadastro será exibido | Formulário de cadastro foi exibido |
|  | Preencher os campos obrigatórios com informações válidas |  Todos os campos são preenchidos com dados digitáveis, onde campo "senha”recebe apenas letras minúsculas |  Todos os campos foram preenchidos com dados digitáveis, onde campo "senha”recebeu apenas letras minúsculas |
|  | Marcar o campo de "Li e concordo com termos de uso” | O campo deve ficar marcado de branco para azul | O campo ficou marcado de branco para azul |
|  | Marcar o campo de “tenho mais de 18 anos” | O campo deve ficar marcado de branco para azul | O campo ficou marcado de branco para azul |
|  | Clicar no botão “cadastrar” | O sistema apresenta o campo “senha” em vermelho e sinaliza também em vermelho os dados obrigatórios para o campo “senha”, neste caso letras maiúsculas, números e caracteres especiais. Pessoa usuária não é registrada. | O sistema apresentou o campo “senha” em vermelho e sinaliza também em vermelho os dados obrigatórios para o campo “senha”, neste caso letras maiúsculas, números e caracteres especiais. Pessoa usuária não é registrada. |

**Teste 5**

![CT5.gif](Criar%20casos%20de%20testes%20para%20o%20fluxo%20de%20cadastro%20da%20/CT5.gif)