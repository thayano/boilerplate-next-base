# Boilerplate Básico Next.js

Este é um boilerplate básico para iniciar projetos Next.js com algumas ferramentas e configurações essenciais já inclusas. Ele visa fornecer uma base sólida para desenvolvimento rápido e organizado.

## O que está incluído?

Este boilerplate já vem configurado com as seguintes dependências e ferramentas de desenvolvimento:

**Dependências:**

- **Next.js (versão 15.3.1)**
- **React (versão 19.0.0)**
- **Tailwind (versão 4)**

**Ferramentas de Desenvolvimento:**

- **TypeScript (versão 5.8.3)**
- **ESLint (versão 9):** Um linter para identificar e corrigir problemas de estilo e erros no seu código JavaScript/TypeScript.
    - **@typescript-eslint/eslint-plugin (versão 8.31.0) e @typescript-eslint/parser (versão 8.31.0):** Suporte do ESLint para TypeScript.
    - **eslint-plugin-next (versão 0.0.0):** Regras adicionais específicas para Next.js no ESLint.
    - **eslint-plugin-tailwindcss (versão 3.18.0):** Plugin do ESLint para garantir boas práticas com Tailwind CSS.
- **Prettier (versão 3.5.3):** Um formatador de código para manter um estilo consistente em todo o projeto.
    - **prettier-plugin-tailwindcss (versão 0.6.11):** Plugin do Prettier para ordenar as classes Tailwind CSS automaticamente.
- **Tailwind CSS (versão 4):** Um framework CSS utilitário para prototipagem e desenvolvimento rápido.
    - **@tailwindcss/postcss (versão 4):** Plugin PostCSS para integrar o Tailwind CSS.
    - **tw-animate-css (versão 1.2.8):** Uma coleção de animações prontas para usar com Tailwind CSS.
- **Husky (versão 9.1.7):** Permite usar Git hooks facilmente.
- **lint-staged (versão 15.5.1):** Executa linters em arquivos staged (antes do commit).

## Scripts NPM

Os seguintes scripts estão configurados no `package.json` para facilitar o desenvolvimento:

- `dev`: Inicia o servidor de desenvolvimento do Next.js com o Turbopack para builds mais rápidos.
- `build`: Executa as verificações do Prettier e, em seguida, builda a aplicação Next.js para produção.
- `start`: Inicia o servidor Next.js em modo de produção.
- `format`: Formata todos os arquivos do projeto usando o Prettier.
- `lint`: Executa o ESLint para verificar problemas de linting no código.
- `check`: Executa apenas a verificação do Prettier para ver se algum arquivo precisa ser formatado.
- `build:local`: Formata os arquivos com Prettier e depois builda a aplicação (útil para builds locais de produção).
- `prepare`: Configura o Husky para os Git hooks.

## Como usar

1.  **Clonar o repositório:**

    ```bash
    git clone [https://docs.github.com/articles/referencing-and-citing-content](https://docs.github.com/articles/referencing-and-citing-content)
    cd boilerplate-next-base
    ```

2.  **Instalar as dependências:**

    ```bash
    npm install
    # ou
    yarn install
    # ou
    pnpm install
    ```

3.  **Iniciar o servidor de desenvolvimento:**

    ```bash
    npm run dev
    # ou
    yarn dev
    # ou
    pnpm dev
    ```

    Abra [http://localhost:3000](http://localhost:3000) no seu navegador para ver a aplicação em execução.

4.  **Buildar a aplicação para produção:**

    ```bash
    npm run build
    # ou
    yarn build
    # ou
    pnpm build
    ```

5.  **Iniciar a aplicação em modo de produção:**
    ```bash
    npm run start
    # ou
    yarn start
    # ou
    pnpm start
    ```

## Configurações Adicionais

- **Tailwind CSS:** A configuração do Tailwind CSS pode ser encontrada no arquivo `tailwind.config.ts` e os estilos globais em `styles/globals.css`.
- **ESLint:** As regras do ESLint estão configuradas no arquivo `.eslintrc.js`.
- **Prettier:** As opções de formatação do Prettier estão no arquivo `.prettierrc.js`.
- **Git Hooks (Husky e lint-staged):** O Husky está configurado para executar o Prettier em arquivos staged antes do commit, garantindo a consistência do código. As configurações do `lint-staged` estão no arquivo `.lintstagedrc.js`.
