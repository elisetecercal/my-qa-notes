# Tela Inicial - Cadastro de Nova PU

Critérios de Aceite: https://miro.com/app/board/uXjVNmWH66w=/?moveToWidget=3458764581387939542\&cot=10 Prioridade: ⭐️⭐️⭐️⭐️⭐️ Severidade: Alta Status: Done Tipo de Bug: Redirecionamento Tipo de Teste: Funcional

| ID                                                                                    | Caso de Teste                                        | Resultados Esperados                                                                                                                                                      | Resultados Obtidos                                                                                                        | Passou ou Nao Passou |
| ------------------------------------------------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | -------------------- |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Botão "Criar Conta”                                  | A nova PU será redirecionado para formulário de cadastro                                                                                                                  | A nova PU foi redirecionada para formulário de cadastro                                                                   | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Criar conta com dados válidos                        | Realizar pre cadastro na aplicação e deve ser exibida mensagem de verificação de e-mail                                                                                   | O sistema realizou a criação do pre cadastro da nova PU. O sistema exibiu mensagem de verificação de e-mail               | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Criar conta com dados inválido                       | Não será realizado o pre-cadastro da nova PU e mensagens em vermelho abaixo dos campos com dados incorretos será exibida                                                  | O sistema não realizou a criação do pre cadastro da nova PU.                                                              |                      |
| O sistema exibiu mensagens em vermelho abaixo dos campos com dados                    | Passou                                               |                                                                                                                                                                           |                                                                                                                           |                      |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Criar conta com dados ja cadastrados                 | Não será realizado o pre-cadastro da nova PU e a mensagem em vermelho acima do botão Cadastrar “Ja existe um usuário cadastrado com esse endereço de e-mail” será exibida | A mensagem em vermelho acima do botão Cadastrar “Ja existe um usuário cadastrado com esse endereço de e-mail” foi exibida | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Criar conta com dados vazios                         | Não será realizado o cadastro e mensagens em vermelho abaixo todos os campos será exibida                                                                                 | O pre-cadastro não foi realizado e mensagens em vermelho abaixo todos os campos foi exibida                               | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Criar conta dados faltantes ( “Nome” e “Sobrenome”.) | Não será realizado o cadastro e mensagens em vermelho abaixo dos campos com dados faltantes será exibida                                                                  | O pre-cadastro não foi realizado e mensagens em vermelho abaixo dos campos com dados faltantes foi exibida                | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md  | Link de verificação de e-mail                        | Link de verificação de e-mail será envia para a nova PU                                                                                                                   | Link de verificação de e-mail recebido com sucesso pela nova PU                                                           | Passou               |
| Tela%20Inicial%20-%20Cadastro%20de%20Nova%20PU%20345664d6f82642dd9723895e0aa1b174.md8 | Realizar Login com PU cadastrada                     | Realizará login com sucesso                                                                                                                                               | O sistema realizou login com sucesso                                                                                      | Passou               |

***

***

**CT001 - Botão “Criar conta”**

* **Nome do caso de Teste: Botão “Criar conta”**
* **Objetivo:** Verificar se o botão “Criar conta” redireciona a nova PU para o formulário de cadastro
* **Pré-condições:** 1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)

2. A nova PU deverá identificar o botão “Criar uma conta”;

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. A nova PU devera visualizar o formulário de cadastro.

* **Resultados esperados:**

1. O sistema deverá redirecionar para a tela de cadastro;

* **Resultados obtido:**
  1. O sistema redirecionou para a tela de cadastro;

***

***

**CT002 - Criar conta com dados validos**

* **Nome do caso de Teste:** Realizar Cadastro
* **Objetivo:** Verificar se é possível realizar novo cadastro no site.
* **Pré-condições:**

1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2. A nova PU deverá identificar o botão “Criar uma conta”;
3. A nova PU não deve ter conta cadastrada em seu e-mail.

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. Inserir nome no campo “Nome civil ou social”, Ex: Elisete;
3. Inserir Sobrenome no campo “Sobrenome”, Ex: Cercal;
4. Inserir e-mail válido no padrão e-mail, Ex: elisetecerca@gmail.com;
5.  Inserir senha no campo “Senha”, seguindo os criterios abaixo, Ex: Elisete@123#;

    **A senha deve conter, no mínimo:**

    **8 caracteres**

    **Letra maiúscula,**

    **Letra minúscula**

    **Número**

    **Caractere especial (ex: #!\*-\_&)**
6. Repetir a senha no campo “Confirme sua senha”: Ex: Elisete@123#;
7. Marcar a check-box “ Li e concordo com os Termos de uso e Politica de Privacidade”;
8. Marcar a check-box “Tenho 18 anos ou mais”;
9. Clicar em Cadastrar.

* **Resultados esperados:**

1. O sistema deverá realizar a criação do novo usuário;
2. O sistema deverá exibir mensagem de verificação de e-mail;

* **Resultados obtidos:**

1. O sistema realizou a criação do novo usuário;
2. O sistema exibiu mensagem de verificação de e-mail

***

***

**CT003 - Criar conta com dados invalido**

* **Nome do caso de Teste:** Realizar Cadastro com dados Inválidos.
* **Objetivo:** Verificar se é possível realizar novo cadastro no site utilizando dados inválidos.
* **Pré-condições:**

1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2.  A nova PU deverá identificar o botão “Criar uma conta”;

    3.A nova PU deverá inserir dados inválidos nos campos imput.

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. Inserir nome no campo “Nome civil ou social”, Ex: Teste;
3. Inserir Sobrenome no campo “Sobrenome”, Ex: Cadeira;
4. Inserir e-mail válido no padrão e-mail, Ex: testecadeira@gmail;
5. Inserir senha no campo “Senha”, seguindo os criterios abaixo, Ex: Test1234;
6. Repetir a senha no campo “Confirme sua senha”: Ex: Test12345;
7. Marcar a check-box “ Li e concordo com os Termos de uso e Politica de Privacidade”;
8. Marcar a check-box “Tenho 18 anos ou mais”;
9. Clicar em Cadastrar.

* **Resultados esperados:**

1. O sistema não deverá realizar a criação do novo usuário;
2. O sistema deverá exibir mensagens em vermelho abaixo dos campos com dados incorretos.

* **Resultados obtidos:**

1. O sistema não realizou a criação do novo usuário;
2. O sistema exibiu mensagem em vermelho abaixo dos campos com dados incorretos.

***

***

***

**CT004 - Criar conta com dados j**á **cadastrados**

* **Nome do caso de Teste:** Realizar Cadastro com dados já cadastrados.
* **Objetivo:** Verificar se é possível realizar novo cadastro no site utilizando dados de uma PU ja cadastrada.
* **Pré-condições:**

1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2.  A nova PU deverá identificar o botão “Criar uma conta”;

    3.A nova PU deverá inserir dados ja cadastrados por outro usuario existente nos campos obrigatorios.

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. Inserir nome no campo “Nome civil ou social”, Ex: Teste;
3. Inserir Sobrenome no campo “Sobrenome”, Ex: Cadeira;
4. Inserir e-mail válido no padrão e-mail, Ex: testecadeira@gmail.com;
5. Inserir senha no campo “Senha”, seguindo os criterios abaixo, Ex: ZxWs6\*asaK$3hk;
6. Repetir a senha no campo “Confirme sua senha”: Ex: ZxWs6\*asaK$3hk;
7. Marcar a check-box “ Li e concordo com os Termos de uso e Politica de Privacidade”;
8. Marcar a check-box “Tenho 18 anos ou mais”;
9. Clicar em Cadastrar.

* **Resultados esperados:**

1. O sistema não deverá realizar a criação do novo usuário;
2. O sistema deverá exibir um mensagem em vermelho acima do botão Cadastrar “Ja existe um usuario cadastrado com esse endereço de e-mail”

* **Resultados obtidos:**

1. O sistema não realizou a criação do novo usuário;
2. O sistema exibiu um mensagem em vermelho acima do botão Cadastrar “Ja existe um usuario cadastrado com esse endereço de e-mail”

***

***

**CT005 - Criar conta com dados vazios**

* **Nome do caso de Teste:** Realizar Cadastro com campos de dados vazios.
* **Objetivo:** Verificar se é possível realizar novo cadastro no site utilizando dados vazios.
* **Pré-condições:**

1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2.  A nova PU deverá identificar o botão “Criar uma conta”;

    3.A nova PU não deverá inserir dados nos campos obrigatorios.

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. Inserir nome no campo “Nome civil ou social”, Ex: ;
3. Inserir Sobrenome no campo “Sobrenome”, Ex: ;
4. Inserir e-mail válido no padrão e-mail, Ex: ;
5. Inserir senha no campo “Senha”, seguindo os criterios abaixo, Ex: ;
6. Repetir a senha no campo “Confirme sua senha”: Ex: ;
7. Marcar a check-box “ Li e concordo com os Termos de uso e Politica de Privacidade”;
8. Marcar a check-box “Tenho 18 anos ou mais”;
9. Clicar em Cadastrar.

* **Resultados esperados:**

1. O sistema não deverá realizar a criação do novo usuário;
2. O sistema deverá exibir mensagens em vermelho abaixo de todos os campos com dados vazios.

* **Resultados obtidos:**

1. O sistema não realizou a criação do novo usuário;
2. O sistema exibiu mensagem em vermelho abaixo de todos os campos com dados vazios.

***

***

CT006 - Criar conta dados faltantes ( “Nome” e “Sobrenome”)

* **Nome do caso de Teste:** Realizar Cadastro com campos de dados faltantes.
* **Objetivo:** Verificar se é possível realizar novo cadastro no site não inserindo todos os dados obrigatorios.
* **Pré-condições:**

1. A nova PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2.  A nova PU deverá identificar o botão “Criar uma conta”;

    3.A nova PU não deverá inserir dados nos campos obrigatorios “Nome” e “Sobrenome”.

* **Passos:**

1. Clicar no botão de “Criar uma conta”;
2. Inserir nome no campo “Nome civil ou social”, Ex: ;
3. Inserir Sobrenome no campo “Sobrenome”, Ex: ;
4. Inserir e-mail válido no padrão e-mail, Ex: testecadeira@gmail.com;
5. Inserir senha no campo “Senha”, seguindo os criterios abaixo, Ex: Teste@1234;
6. Repetir a senha no campo “Confirme sua senha”: Ex: Teste@1234;
7. Marcar a check-box “ Li e concordo com os Termos de uso e Politica de Privacidade”;
8. Marcar a check-box “Tenho 18 anos ou mais”;
9. Clicar em Cadastrar.

* **Resultados esperados:**

1. O sistema não deverá realizar a criação do novo usuário;
2. O sistema deverá exibir mensagens em vermelho abaixo dos campos “Nome” e “Sobrenome” com dados vazios .

* **Resultados obtidos:**

1. O sistema não realizou a criação do novo usuário;
2. O sistema exibiu mensagem em vermelho abaixo de dos os campos “Nome” e “Sobrenome” com dados vazios.

***

***

CT007 - Link de verificação de e-mail para nova PU

**Nome do caso de Teste:** Envio de link de verificação de e-mail para nova PU e conclusão de cadastro da nova PU

* **Objetivo:** Concluir cadastro da nova PU na aplicação LS através do link de confirmação de e-mail e seleção de dados pessoais no pós-cadastro.
* **Pré-condições:**

1. A nova PU deverá ter preenchido com sucesso o formulario do link : [https://paciente.lacreisaude.com.br/cadastro/](https://paciente.lacreisaude.com.br/cadastro/)2. A PU deverá ter acesso a caixa de e-mail pré-cadastrado na aplicação LS;

* **Passos:**

1. Receber o link de verificação de e-mail em sua caixa de entrada (se realizou o preenchimento do formulário de pré-cadastro de maneira correta);
2. Clicar no link que a redicionará para a pagina de “Login”;
3. Inserir dados de login e clicar no botão “Entrar”.
4. Será redirecionada para página de “Continuar Cadastro”
5. PU poderá selecionar mais dados pessoais através das caixas de seleção disponíveis;
6. Ao final desta seleção poderá selecionar “Buscar de Profissionais” ou “Editar”;

* **Resultados esperados:**

1. O sistema deverá enviar o de verificação link para o e-mail cadastrado da nova PU;
   1. O link enviado deverá redirecionar a nova PU para a página de login;
   2. A nova PU deverá realizar o login com sucesso
   3. A nova PU deve concluir o seu pós-cadastro com sucesso e poderá visualizar a página de “Busca por profissionais ” como esperado.

* **Resultados obtidos:**

1. O sistema enviou link com sucesso;
   1. O link enviado redirecionou a nova PU para a página de login como esperado;
   2. A nova PU realizou login com sucesso;
   3. A nova PU concluiu seu pós-cadastro com sucesso e pode visualizar a página de “Busca por profissionais ” como esperado.

***

***

CT008 - Realizar Login com PU cadastrada na LS

* **Nome do caso de Teste:** Realizar Login de PU cadastrada
* **Objetivo:** Verificar se é possível realizar login com PU válido cadastrado na aplicação LS
* **Pré-condições:**

1. A PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/)
2.  A PU deverá estar cadastrada na aplicação LS;

    3.A PU deverá inserir os dados corretos para realizar login com sucesso.

* **Passos:**

1. Inserir e-mail válido em formato padrão e-mail, Ex: testecadeira@gmail.com;
2. Inserir senha cadastrada na sua conta, no campo “Senha”, Ex: ZxWs6\*asaK$3hk;
3. Clicar no botão “Entrar”.
4. Será redirecionada para página de “Busca profissional”
5. PU terá acesso aos links rápidos de Perfil, Ajuda, Sair e Interprete de libra simultâneo.

* **Resultados esperados:**

1. O sistema realizará o login com sucesso e o direcionará a PU para a página de Busca Profissional;

* **Resultados obtidos:**

1. O sistema realizou login com sucesso;
