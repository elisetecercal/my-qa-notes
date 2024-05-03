# Esquecer a senha da pessoa usuária

Critérios de Aceite: https://miro.com/app/board/uXjVNmWH66w=/?moveToWidget=3458764581406111073\&cot=10 Prioridade: ⭐️⭐️⭐️ Severidade: Alta Status: Done Tipo de Teste: Funcional

| ID                                                                                       | Caso de Teste                        | Resultados Esperados                                                                                                                      | Resultados Obtidos                                                 | Passou ou Não Passou |
| ---------------------------------------------------------------------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------- |
| Esquecer%20a%20senha%20da%20pessoa%20usua%CC%81ria%205c431126c5324de9adc76f708a9e62ed.md | Recuperar password com user válido   | Alteração da senha será realizada com sucesso                                                                                             | A alteração aconteceu com sucesso                                  | Passou               |
| Esquecer%20a%20senha%20da%20pessoa%20usua%CC%81ria%205c431126c5324de9adc76f708a9e62ed.md | Recuperar password com user inválido | Mensagem de :” Por favor, utilize um formato de e-mail válido. Por exemplo: mailto:email@dominio.com.br.” e a alteração não será possivel | A mensagem foi exibida com sucesso e a senha não pode ser alterada | Passou               |
| CT015                                                                                    | Recuperar password com user excluido | Alteração não poderá acontecer                                                                                                            | Não obtive resultado suficiente                                    | Não Passou           |

CT013 - Recuperar password com user válido

* **Nome do caso de Teste:** Recuperar password com user válido
* **Objetivo:** Verificar se o fluxo de recuperação de senha acontece com sucesso
* **Pré-condições:**

1. A PU deverá ter cadastro ativo na aplicação LS
2. A PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/redefinicao-de-senha/](https://paciente.lacreisaude.com.br/redefinicao-de-senha/)
3. A PU deve ter acesso ao e-mail informado para a recuperação da senha

* **Passos:**

1. Identificar campo input “**E-mail**”;
2. Inserir e-mail cadastrado em sua conta LS. Ex: testcadeiraqa@gmail.com;
3. Clicar no botão “Enviar link”;
4. Visualizar a mensagem de “ Verifique seu e-mail para redefinir a senha. Caso o e-mail fornecido exista, será enviado um link para redefinição de senha. Por favor, clique em reenviar se não receber o link.”.
5. Clicar no link enviado para o e-mail indicado;
6. Ser redirecionado para a pagina “Cadastre uma nova senha”
7. Inserir nova senha nos campos “Nova Senha” e “Repetir Senha” obedecendo os criterios abaixo:
   * 8 caracteres
   * Letra maiúscula
   * Letra minúscula
   * Número
   * Caractere especial(exemplo: #!\*-\_&)
   * As senhas devem ser iguais
8. Clicar em redefinir senha;
9. Mensagem de “Senha alterada com sucesso”, deverá ser exibida.

Resultado esperado

1. A senha será alterada com sucesso;

* **Resultados obtido:**
  1. A senha foi alterada com sucesso

***

***

***

CT014 - Recuperar password com user inválido

* **Nome do caso de Teste:** Recuperar password com user inválido
* **Objetivo:** Verificar se o sistema identifica um e-mail fora do padrão
* **Pré-condições:**

1. A PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/redefinicao-de-senha/](https://paciente.lacreisaude.com.br/redefinicao-de-senha/)

* **Passos:**

1. Identificar campo input “**E-mail**”;
2. Inserir e-mail no campo input. Ex: eli@emailcom;
3. Clicar no botão “Enviar link”;
4. Visualizar a mensagem de “ Por favor, utilize um formato de e-mail válido. Por exemplo: [email@dominio.com.br](mailto:email@dominio.com.br).”.

Resultado esperado

1. O sistema deve exibir mensagem de erro abaixo do campo e-mail;

*   **Resultados obtido:**

    1. O sistema exibiu mensagem de erro abaixo do campo e-mail;

    ***

    ***

    CT015 - Recuperar password com user excluido

    * **Nome do caso de Teste:** Recuperar password com user excluido
    * **Objetivo:** Verificar se o sistema identifica que o e-mail utilizado ja não esta mais cadastrado na aplicação.
    * **Pré-condições:**
    * A PU deverá estar no link do site: [https://paciente.lacreisaude.com.br/redefinicao-de-senha/](https://paciente.lacreisaude.com.br/redefinicao-de-senha/)
    * E-mail utilizado deve ter sido excluido atraves do formulário “Apagar minha conta”.
    * **Passos:**
    * Identificar campo input “**E-mail**”;
    * Inserir e-mail no campo input. Ex: testcadeira@gmail.com;
    * Clicar no botão “Enviar link”;
    * Visualizar a mensagem de “Verifique seu e-mail para redefinir a senha. Caso o e-mail fornecido exista, será enviado um link para redefinição de senha. Por favor, clique em reenviar se não receber o link.”
    * Não deve ser enviado link para o e-mail que esta excluido do sistema

    Resultado esperado

    1. O sistema deve exibir mensagem “Verifique seu e-mail para redefinir a senha. Caso o e-mail fornecido exista, será enviado um link para redefinição de senha. Por favor, clique em reenviar se não receber o link.”
    2. **Resultados obtido:**
       1. Não foi possivel realizar este teste por motivo de não conclusão do processo de exclusão da conta cadastrada, o e-mail com a solicitação não havia chego ate a conclusão deste desafio.
