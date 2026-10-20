# Automação E2E com Cypress — Swag Labs

Projeto de portfólio para praticar testes end-to-end (E2E) em uma loja virtual de demonstração: [Swag Labs](https://www.saucedemo.com/).

## Objetivo

Automatizar fluxos importantes de uma compra online, validando comportamentos esperados e algumas situações de erro.

## Tecnologias

- JavaScript
- Cypress
- Node.js e npm
- Git e GitHub

## Cenários automatizados

1. Login com credenciais válidas.
2. Mensagem de erro ao informar senha incorreta.
3. Bloqueio de acesso para usuário bloqueado.
4. Adição de produto ao carrinho.
5. Checkout completo com dados válidos.
6. Validação de campo obrigatório no checkout.

## Pré-requisitos

- Node.js em versão LTS instalada.
- npm (incluído com o Node.js).
- Acesso à internet para abrir o Swag Labs e instalar as dependências.

## Como executar

Abra o terminal na pasta `projeto-cypress-swag-labs` e execute:

```bash
npm install
```

Para abrir a interface do Cypress:

```bash
npm run cy:open
```

Na janela do Cypress, selecione **E2E Testing**, escolha um navegador e execute `swag-labs.cy.js`.

Para executar os testes no terminal, em modo headless:

```bash
npm run cy:run
```

Se o Google Chrome estiver instalado, também é possível executar:

```bash
npm run cy:chrome
```

## Usuários de demonstração

O Swag Labs disponibiliza contas de teste na própria tela de login. Este projeto usa:

- Usuário válido: `standard_user`
- Usuário bloqueado: `locked_out_user`
- Senha de demonstração: `secret_sauce`

Use essas credenciais apenas no site de demonstração.

## Estrutura

```text
projeto-cypress-swag-labs/
├── cypress/
│   └── e2e/
│       └── swag-labs.cy.js
├── .gitignore
├── cypress.config.js
├── package.json
└── README.md
```

## Observações

- Os testes dependem da disponibilidade do site público de demonstração.
- O projeto foi preparado como base de estudo. Execute os testes no seu computador e confira os resultados antes de apresentar a execução como validada.
- Os dados preenchidos no checkout são fictícios.

## Autoria

Projeto desenvolvido para compor meu portfólio de Engenharia de Qualidade de Software.

**Perfil GitHub:** [priottomarcos7-coder](https://github.com/priottomarcos7-coder)
