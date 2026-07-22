# Guia de Contribuição

Obrigada por considerar contribuir com o projeto **Front-end na Vida Real**!

Este documento apresenta o padrão utilizado para criação de branches, commits e pull requests.

## Como contribuir

### 1. Faça um fork

Crie uma cópia do repositório na sua conta do GitHub utilizando a opção **Fork**.

### 2. Clone o repositório

```bash
git clone https://github.com/SEU-USUARIO/Front-end_na_vida_real.git
```

Entre na pasta do projeto:

```bash
cd Front-end_na_vida_real/csshortcut-app
```

### 3. Instale as dependências

```bash
npm install
```

Caso ainda não tenha o Gulp CLI instalado:

```bash
npm install -g gulp-cli
```

### 4. Atualize a branch principal

Antes de começar uma alteração, volte para a branch `main` e atualize o projeto:

```bash
git checkout main
git pull origin main
```

Não realize alterações diretamente na branch `main`.

## Padrão de branches

As branches devem seguir este formato:

```text
tipo/descricao-da-alteracao
```

A descrição deve:

* utilizar letras minúsculas;
* não possuir espaços;
* não possuir acentos;
* separar as palavras com hífen;
* explicar brevemente a alteração.

### Tipos de branch

| Tipo       | Quando utilizar                                  | Exemplo                                 |
| ---------- | ------------------------------------------------ | --------------------------------------- |
| `feat`     | Criação de uma nova funcionalidade               | `feat/adiciona-menu-mobile`             |
| `fix`      | Correção de um erro                              | `fix/corrige-link-do-header`            |
| `docs`     | Alterações na documentação                       | `docs/atualiza-readme`                  |
| `style`    | Alterações visuais ou de formatação              | `style/ajusta-espacamento-do-card`      |
| `refactor` | Melhoria no código sem alterar seu comportamento | `refactor/reorganiza-funcoes`           |
| `test`     | Criação ou alteração de testes                   | `test/adiciona-teste-do-menu`           |
| `chore`    | Tarefas de manutenção e configuração             | `chore/atualiza-dependencias`           |
| `hotfix`   | Correção urgente de um problema importante       | `hotfix/corrige-carregamento-da-pagina` |

### Criando uma branch

Exemplo para uma nova funcionalidade:

```bash
git checkout -b feat/adiciona-menu-mobile
```

Exemplo para uma correção:

```bash
git checkout -b fix/corrige-link-do-header
```

Exemplo para documentação:

```bash
git checkout -b docs/atualiza-readme
```

## Padrão de commits

Os commits devem seguir este formato:

```text
tipo: descricao da alteracao
```

Utilize uma descrição curta e objetiva, informando o que foi alterado.

### Tipos de commit

| Tipo       | Quando utilizar                          |
| ---------- | ---------------------------------------- |
| `feat`     | Nova funcionalidade                      |
| `fix`      | Correção de erro                         |
| `docs`     | Alteração na documentação                |
| `style`    | Alteração visual ou de formatação        |
| `refactor` | Refatoração sem mudança de comportamento |
| `test`     | Criação ou alteração de testes           |
| `chore`    | Manutenção, configuração ou dependências |

### Exemplos

```bash
git commit -m "feat: adiciona menu mobile"
```

```bash
git commit -m "fix: corrige alinhamento do cabecalho"
```

```bash
git commit -m "docs: atualiza instrucoes de instalacao"
```

```bash
git commit -m "style: ajusta espacamento dos botoes"
```

```bash
git commit -m "refactor: reorganiza funcoes do projeto"
```

```bash
git commit -m "chore: atualiza dependencias"
```

Evite mensagens genéricas como:

```text
alteracoes
ajustes
correcao
commit novo
finalizado
```

## Executando o projeto

Para iniciar o servidor de desenvolvimento:

```bash
npm start
```

Para gerar os arquivos finais do projeto:

```bash
npm run build
```

Antes de enviar sua contribuição, verifique se o projeto continua funcionando corretamente.

## Enviando as alterações

Confira os arquivos modificados:

```bash
git status
```

Adicione as alterações:

```bash
git add .
```

Crie o commit:

```bash
git commit -m "feat: adiciona nova funcionalidade"
```

Envie a branch para o GitHub:

```bash
git push -u origin feat/adiciona-nova-funcionalidade
```

## Criando um Pull Request

Depois de enviar a branch:

1. Acesse o repositório no GitHub.
2. Clique em **Compare & pull request**.
3. Selecione a branch `main` como destino.
4. Adicione um título objetivo.
5. Explique as alterações realizadas.
6. Envie o Pull Request.

### Padrão do título

O título do Pull Request deve seguir o mesmo padrão dos commits:

```text
feat: adiciona menu mobile
```

```text
fix: corrige alinhamento do cabecalho
```

```text
docs: atualiza guia de contribuicao
```

### Descrição sugerida

```markdown
## O que foi alterado?

Descreva brevemente as alterações realizadas.

## Por que essa alteração foi necessária?

Explique o problema resolvido ou a melhoria adicionada.

## Como testar?

Informe os passos necessários para testar a alteração.

## Checklist

- [ ] Testei as alterações localmente.
- [ ] O projeto continua funcionando corretamente.
- [ ] Não alterei arquivos que não fazem parte da tarefa.
- [ ] Revisei o código antes de enviar.
- [ ] Segui o padrão de branches e commits.
```

Caso o Pull Request resolva uma issue, adicione na descrição:

```text
Closes #numero-da-issue
```

Exemplo:

```text
Closes #3
```

## Boas práticas

* Mantenha cada branch focada em apenas uma tarefa.
* Evite misturar correções e funcionalidades diferentes.
* Faça commits pequenos e objetivos.
* Não envie a pasta `node_modules`.
* Revise o código antes de criar o Pull Request.
* Mantenha o padrão de organização já utilizado no projeto.
* Explique claramente o motivo das alterações.
* Aguarde a revisão antes de excluir a branch.

## Depois da aprovação

Após o Pull Request ser aprovado e integrado à branch `main`, a branch utilizada pode ser removida:

```bash
git branch -d nome-da-branch
```

Para remover a branch do repositório remoto:

```bash
git push origin --delete nome-da-branch
```

Obrigada por contribuir!
