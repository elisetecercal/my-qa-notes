# Registrar os bugs, caso existam, na própria documentação;

**Bug:** Usuário realizou a exclusão de sua conta no sistema através do botão "Apagar minha conta”, ao tentar se registrar novamente uma mensagem de "Um usuário já foi registrado com este endereço de e-mail.” foi exibida, não permitindo que o mesmo realiza-se o cadastro novamente.

**Cenário Conta excluída:** Usuário fornece informações válidas de uma pessoa usuária que havia realizado a exclusão de sua conta.

**Entrada:**

* Nome: Elisete
* Sobrenome: Cercal
* E-mail: elisetecercal@gmail.com
* Senha: Elisete@123

**Saída:** Que o usuário que realizou a exclusão de sua conta consiga realizar um novo cadastro pelo formulário de cadastro.

| Caso de Teste Cadastro de pessoa usuária                                                                         | Passos                                                                                                                                  | Resultado esperado                                                               | Resultado Teste                              |
| ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------- |
| CTCE: Usuário fornece informações válidas de uma pessoa usuária que realizou a exclusão de sua conta no sistema. | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/                                                                | Página home será exibida “Bem vinda à Lacrei”                                    | Página home foi exibida “Bem vinda à Lacrei” |
|                                                                                                                  | Clicar no botão “Criar conta”                                                                                                           | Formulário de cadastro será exibido                                              | Formulário de cadastro foi exibido           |
|                                                                                                                  | Preencher os campos obrigatórios com informações válidas                                                                                | Os campos devem receber dados digitados válidos                                  | Os campos receberam dados digitados válidos  |
|                                                                                                                  | Marcar o campo de "Li e concordo com termos de uso”                                                                                     | O campo deve ficar marcado de branco para azul                                   | O campo ficou marcado de branco para azul    |
|                                                                                                                  | Marcar o campo de “tenho mais de 18 anos”                                                                                               | O campo deve ficar marcado de branco para azul                                   | O campo ficou marcado de branco para azul    |
|                                                                                                                  | Clicar no botão “cadastrar”                                                                                                             | O sistema apresenta uma mensagem para confirmação de e-mail “Para sua segurança, |                                              |
| enviamos um link de verificação para o e-mail cadastrado”                                                        | O sistema apresentou uma mensagem “Um usuário já foi registrado com este endereço de e-mail.” Pessoa usuária não foi cadastrada. Falhou |                                                                                  |                                              |

![CTCE.gif](../../Software%20Tests/Plano%20de%20teste/Registrar%20os%20bugs,%20caso%20existam,%20na%20pro%CC%81pria%20docum/CTCE.gif)

***

***

***

**Bug 2:** A pessoa usuária acessa através de um smartphone, na página de “Boas Vindas à Lacrei” todos os campos de login são responsivos nesta página, entre tanto o botão de “Ajuda” que no smartphone se torna um ponto de interrogação “?” quando é clicado não funciona, ou seja, não apresenta a lista de “Perguntas Frequentes".

**Cenário botão de Ajuda smartphone:** Usuário acessa a página “Boas Vindas Lacrei” através de um dispositivo móvel neste caso um smartphone e clica no botão "Ajuda”.

**Entrada:**

* Clicar no botão "Ajuda” utilizando dispositivo móvel.

**Saída:**

* Redirecionamento para a página com a lista de "Perguntas Frequentes”

| Caso de Teste botão de “Ajuda”          | Passos                                                                                            | Resultado Esperado                                                   | Resultado Teste                               |
| --------------------------------------- | ------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | --------------------------------------------- |
| CTBA: Usuário clica no botão de “Ajuda” | Acessar a página home https://frontend-lacrei-pessoa-usuaria.vercel.app/ através de um smartphone | Página home será exibida “Bem vinda à Lacrei”                        | Página home foi exibida “Bem vinda à Lacrei”  |
|                                         | Clicar no botão de “Ajuda” no canto superior direito da tela do smartphone                        | Redirecionamento para a página com a lista de “Perguntas frequentes” | Nada acontece, botão não responde ao comando. |
