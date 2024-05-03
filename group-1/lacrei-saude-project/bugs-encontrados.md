# Bugs encontrados

Critérios de Aceite: Qualquer comportamento não esperado/desejado exibido na aplicação Prioridade: ⭐️⭐️⭐️⭐️⭐️ Severidade: Alta Status: Done Tipo de Teste: Exploratório

| ID                                                       | Bug                                                                         | Observações                                                     | Tipo de Bug            | Reprodutibilidade | Severidade |
| -------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------- | ---------------------- | ----------------- | ---------- |
| Bugs%20encontrados%2002d6e3afb08543dbbd12a1b1b5c59fb1.md | Redirecionamento de Página e Desconexão inesperada da conta                 | Navegador Chrome Version 122.0.6261.94 - MacOs                  | Interface e Funcional  | Sempre            | Alta       |
| Bugs%20encontrados%2002d6e3afb08543dbbd12a1b1b5c59fb1.md | Bug não envio da solicitação de exclusão de conta LS                        | Navegador Chrome Version 122.0.6261.94 (Official Build) (arm64) | Funcional              | Sempre            | Alta       |
| Bugs%20encontrados%2002d6e3afb08543dbbd12a1b1b5c59fb1.md | Redirecionamento de Página exibe tela Branca com texto em tamanho Grande    | Navegador Chrome Version 122.0.6261.94 (Official Build) (arm64) | Interface e desempenho | Sempre            | Baixa      |
| Bugs%20encontrados%2002d6e3afb08543dbbd12a1b1b5c59fb1.md | Redirecionamento de Página exibe tela Branca com texto em tamanho Grande    | Navegador Chrome Version 122.0.6261.94 (Official Build) (arm64) | Interface e desempenho | Sempre            | Baixa      |
| Bugs%20encontrados%2002d6e3afb08543dbbd12a1b1b5c59fb1.md | Redirecionamento de Página a tela gira e as informações carregam lentamente | Navegador Chrome Version 122.0.6261.94 (Official Build) (arm64) | Desempenho             | Intermitente      | Baixa      |

B001 - Redirecionamento de Pagina e Desconexão inesperada da conta

Descrição : O usuário realiza login, navega até a página de buscar profissional, clica no botão "Ajuda" e é redirecionado para a página de "Perguntas frequentes". Em seguida, clica no link para voltar à página "Início", mas ao ser redirecionado para a página de "Início" é deslogado de sua conta. Ao clicar no botão "Para o Paciente", a página para a qual foi redirecionado (tela de login) carrega fora de formatação.

**Passos para reproduzir:**

1. Realize o login na aplicação - [https://paciente.lacreisaude.com.br/](https://paciente.lacreisaude.com.br/).
2. Na página “Buscar Profissionais”, clique no botão “Ajuda”.
3. Será exibido um lista de perguntas frequentes.
4. Clique no link de página, “Início”.
5. Será redirecionado para a página de apresentação da LS- [https://lacreisaude.com.br/](https://lacreisaude.com.br/), e não estará mais ativo como usuário da aplicação.

B002 - Bug não envio da solicitação de exclusão de conta LS

**Descrição:** Preencho um formulário na aplicação web solicitando a exclusão da minha conta, envio clicando em um botão de “Solicitar”. A mensagem de solicitação realizada com sucesso é exibida, mas não recebo o e-mail que deveria ser enviado com a confirmação do meu pedido.

**Passos para reproduzir:**

1. Acesse o formulário na aplicação web - [https://lacreisaude.com.br/direitos-de-titular/](https://lacreisaude.com.br/direitos-de-titular/)
2. Preencha todos os campos do formulário.
3. Clique no botão "Solicitar".
4. A mensagem de solicitação realizada com sucesso é exibida.
5. Verifique sua caixa de entrada de e-mail, mas o e-mail com seus dados não está presente.

```
            Captura de tela e-mail que realizou a solicitação de exclusão de conta.
```

B003 - Redirecionamento de Página exibe tela Branca com texto em tamanho Grande

**Descrição:** Realizei a solicitação de redefinir senha através da aplicação, recebi o e-mail com o link para realizar a redefinição. Quando clico no link sou redirecionada para uma tela branca com letras em tamanho grande e em alguns segundos o formulário de redefinir senha e exibido.

**Passos para reproduzir:**

1. Clique no link de redefinição de senha enviado para o seu e-mail.
2. A tela branca com texto em tamanho grande é exibida por 2 segundos.
3. A página esperada "redefinir senha" é exibida.

B004 - Redirecionamento de Página exibe tela Branca com texto em tamanho Grande

Descrição:

**Passos para reproduzir:**

1. Acesse a página de “Perfil”.
2. Clique no botão “Editar foto”.
3. Será redirecionado para a página “Foto de perfil”
4. Clique em “Enviar foto”.
5. Clique em “Cancelar”.
6. A página ficará Branca com letras de tamanho grande por poucos segundos.

B005 - Redirecionamento de Página a tela gira e as informações carregam lentamente

Descrição: Depois de realizar o login, cliquei no meu perfil e o bug se apresentou girando a tela enquanto carregava lentamente as outras informações da página.

**Passos para reproduzir:**

1. Acesse a página de “Buscar por profissionais”.
2. Clique no link para a página de “Perfil”.
3. A tela gira e as informações carregam lentamente.
