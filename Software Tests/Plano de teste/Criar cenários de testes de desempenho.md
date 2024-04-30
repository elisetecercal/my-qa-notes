# Criar cenários de testes de desempenho

Os testes de desempenho serão realizados utilizando ferramenta JMeter na versão  para os seguintes cenários.

## **Cenário 1**

Teste de carga para o fluxo de cadastro da pessoa usuária

**Entrada:**

- 100 usuários
- Cada usuário realiza 10 tentativas de cadastro

**Saída:**

- O sistema deve ser capaz de lidar com as solicitações sem falhas ou lentidão.

**Expectativa:**

- O sistema deve registrar com sucesso 100 usuários.

[lacrei-saude.pagina-de-login.csv](Criar%20cena%CC%81rios%20de%20testes%20de%20desempenho/lacrei-saude.pagina-de-login.csv)

## **Cenário 2**

Teste de desempenho para o fluxo de login da pessoa usuária

Teste de estresse para o fluxo de login da pessoa usuária

**Entrada:**

- 100 usuários
- Cada usuário realiza 2 tentativas de login

**Saída:**

- O sistema deve ser capaz de lidar com as solicitações sem falhas ou lentidão.

**Expectativa:**

- O sistema deve autenticar com sucesso 100 usuários.

[lacrei-saude.pagina-de-cadastro.csv](Criar%20cena%CC%81rios%20de%20testes%20de%20desempenho/lacrei-saude.pagina-de-cadastro.csv)