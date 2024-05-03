# Criar cenários de testes de responsividade mobile considerando dois tipos de dispositivos

Os testes de responsividade mobile também foram realizados através da ferramenta Mobile -Friendly da Google, onde se apresentou o resultado de que a pagina [https://frontend-lacrei-pessoa-usuaria.vercel.app/cadastro](https://frontend-lacrei-pessoa-usuaria.vercel.app/cadastro) é responsiva e de fácil utilização em um dispositivo móvel.

T**este de responsividade mobile para o fluxo de cadastro da pessoa usuária**

## **Cenário1**

Teste de visualização para o formulário de cadastro da pessoa usuária em um smartphone (iphone13) utilizando o aplicativo de captura de tela nativo do aparelho

**Entrada:**

* Formulário de cadastro da pessoa usuária
* Smartphone (Iphone13)

**Saída:**

* O formulário deve ser visualmente agradável em um smartphone.

**Expectativa:**

* Os campos do formulário devem ser legíveis e fáceis de usar.

| Caso de Teste Cadastro de pessoa usuária utilizando smartphone (iphone 13) | Passos                                                                                                                       | Resultado esperado                                                                | Resultado Teste                                                                        |
| -------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| CT1: Usuário fornece informações válidas.                                  | Acessar a pagina home https://frontend-lacrei-pessoa-usuaria.vercel.app/ através do smartphone                               | Página home será exibida “Bem vinda à Lacrei”                                     | Página home foi exibida “Bem vinda à Lacrei”                                           |
|                                                                            | Clicar no botão “Criar conta”                                                                                                | Formulário de cadastro será exibido                                               | Formulário de cadastro foi exibido                                                     |
|                                                                            | Preencher os campos obrigatórios com informações válidas                                                                     | Os campos devem receber dados digitados e válidos                                 | Os campos receberam dados digitados e válidos                                          |
|                                                                            | Marcar o campo de "Li e concordo com termos de uso”                                                                          | O campo deve ficar marcado de branco para verde                                   | O campo ficou marcado de branco para verde                                             |
|                                                                            | Marcar o campo de “tenho mais de 18 anos”                                                                                    | O campo deve ficar marcado de branco para verde                                   | O campo ficou marcado de branco para verde                                             |
|                                                                            | Clicar no botão “cadastrar”                                                                                                  | O sistema apresenta uma mensagem para confirmação de e-mail “Para sua segurança,  |                                                                                        |
| enviamos um link de verificação para o e-mail cadastrado”                  | Sistema apresentou mensagem “Um usuário já foi cadastrado com este e-mail”                                                   |                                                                                   |                                                                                        |
|                                                                            | Após o recebimento do link de verificação na caixa de e-mail da nova pessoa cadastrada, clicar no link para confirmar e-mail | O sistema apresenta uma menssagem para confirmação de e-mail “Para sua segurança, |                                                                                        |
| enviamos um link de verificação para o e-mail cadastrado”                  | N/A                                                                                                                          |                                                                                   |                                                                                        |
| Conclusão                                                                  |                                                                                                                              |                                                                                   | O formulário é visualmente agradável em um smartphone, de fácil navegação e intuítivo. |

teste-responsivo-iphone-crie.mov

## Cenário 2

Teste de responsividade mobile para o fluxo de login da pessoa usuária em um tablet

Cenário de teste:

Teste de funcionalidade para o formulário de login da pessoa usuária em um tablet

**Entrada:**

* Formulário de login da pessoa usuária
* Tablet

**Saída:**

* O formulário deve ser funcional em um tablet.
