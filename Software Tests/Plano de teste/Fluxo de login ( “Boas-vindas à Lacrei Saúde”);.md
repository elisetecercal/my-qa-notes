# Fluxo de login ( “Boas-vindas à Lacrei Saúde”);

# **Casos de teste para o fluxo de login da pessoa usuária**

**Escopo:**

O fluxo de login da pessoa usuária deve permitir que uma pessoa usuária já cadastrada faça login no sistema utilizando suas credenciais validas.

# **Cenários**

## **Cenário 1**

Pessoa usuária fornece informações válidas.

**Entrada:**

- E-mail: elisetecercal@gmail.com
- Senha: Elisete@123

**Saída:**

- Pessoa usuária é autenticado com sucesso.

| Caso de Teste Login de pessoa usuária | Passos | Resultado esperado |
| --- | --- | --- |
| CT1: Pessoa usuária fornece informações válidas já cadastradas no sistema. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | Página home será exibida “Bem vinda à Lacrei” |
|  | Preencher os campos obrigatórios com informações válidas já cadastradas | Todos os campos são preenchidos com dados já cadastrados. |
|  | Clicar no botão “Entrar” | O sistema apresenta uma mensagem “Boas-vindas à Lacrei Saúde, continue o seu cadastro”. |

**Teste 1**

![CTL1.gif](Fluxo%20de%20login%20(%20%E2%80%9CBoas-vindas%20a%CC%80%20Lacrei%20Sau%CC%81de%E2%80%9D);/CTL1.gif)

## **Cenário 2**

Pessoa usuária cadastrada fornece informações inválidas para os campos "e-mail ” e "senha” na página "Bem vinda à Lacrei”.

**Entrada:**

- E-mail: elisetecercal@gmail
- Senha:12345678

**Saída:**

Pessoa usuária não é autenticado.

| Caso de Teste Login de pessoa usuária | Passos | Resultado esperado |
| --- | --- | --- |
| CT2: Usuário cadastrado no sistema fornece informações inválidas  | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | Página home será exibida “Bem vinda à Lacrei” |
|  | Preencher os campos de “Login”obrigatórios com informações inválidas de um usuário cadastrado | Todos os campos são preenchidos com dados inválidos, “e-mail” faltando o “.com” e o campo “senha ” com números. |
|  | Clicar no botão “Entrar” | O sistema apresenta uma mensagem “Sua senha e/ou conta está incorreta. Se tiver esquecido a senha, clique em “Esqueci minha senha””. |

**Teste 2**

![CTL2.gif](Fluxo%20de%20login%20(%20%E2%80%9CBoas-vindas%20a%CC%80%20Lacrei%20Sau%CC%81de%E2%80%9D);/CTL2.gif)

## **Cenário 3**

Pessoa usuária cadastrada.

**Entrada:**

- E-mail: jpcercal@gmail.com
- Senha: Jpcercal@123

**Saída:**

Pessoa usuária não é autenticado.

| Caso de Teste Login de pessoa usuária | Passos | Resultado esperado |
| --- | --- | --- |
| CT3: Usuário não esta cadastrado no sistema fornece informações válidas  | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ | Página home será exibida “Bem vinda à Lacrei” |
|  | Preencher os campos obrigatórios de “Login” com informações válidas porém não cadastradas | Todos os campos são preenchidos com dados válidos. |
|  | Clicar no botão “Entrar” | O sistema apresenta uma mensagem “Sua senha e/ou conta está incorreta. Se tiver esquecido a senha, clique em “Esqueci minha senha””. |

**Teste 3**

![CTL3.gif](Fluxo%20de%20login%20(%20%E2%80%9CBoas-vindas%20a%CC%80%20Lacrei%20Sau%CC%81de%E2%80%9D);/CTL3.gif)