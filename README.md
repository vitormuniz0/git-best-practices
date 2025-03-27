# Guia Essencial de Git

Um guia rápido com os comandos Git mais usados e basicos para iniciar e gerenciar seu projeto, com maior foco nas padronizações de commits.

## ⚙️ Comandos Básicos

### Configuração Inicial

```sh

# Configura seu nome de usuário
git config --global user.name "Seu Nome"

# Configura seu email
git config --global user.email "[endereço de email removido]"

# Inicializa um novo repositório Git no diretório atual
git init

# Clona um repositório remoto para sua máquina
git clone <URL_do_repositório>

```

### Alterações e Commits

```sh

# Verifica o status das suas alterações
git status

# Adiciona arquivos para o próximo commit
git add <arquivo> # ou git add . para adicionar tudo

# Cria um commit com uma mensagem descritiva
git commit -m "Mensagem do commit"

```

### Branches

```sh

# Lista todas as branches
git branch

# Cria uma nova branch
git branch <nome-da-branch>

# Muda para uma branch existente
git checkout <nome-da-branch>

# Cria e muda para uma nova branch
git checkout -b <nome-da-branch>

# Mescla alterações de outra branch na branch atual
git merge <nome-da-branch>

```

### Repositórios Remotos

```sh

# Envia commits para o repositório remoto
git push origin <nome-da-branch>

# Baixa as últimas alterações do repositório remoto
git pull origin <nome-da-branch>

```

### Desfazendo Alterações

```sh

# Desfaz alterações em um arquivo antes do commit
git checkout -- <arquivo>

# Desfaz o último commit (mantém as alterações)
git reset --soft HEAD~1

# Desfaz o último commit (descarta as alterações)
git reset --hard HEAD~1

```

# Padronização de Commits

Manter um histórico de commits limpo e organizado é crucial para a colaboração e a manutenção de projetos. Uma padronização de commits ajuda a garantir que cada commit seja claro, conciso e informativo.

## Formato Padrão

A convenção mais comum é seguir o formato:

* **`<tipo>`**: Indica a natureza da mudança.
* **`<mensagem curta>`**: Uma descrição concisa da mudança.

## Tipos de Commits

Aqui estão alguns tipos de commits amplamente utilizados:

* **feat**: Adiciona uma nova funcionalidade.
* **fix**: Corrige um bug.
* **docs**: Atualiza a documentação.
* **style**: Modifica a formatação do código (sem alterar a lógica).
* **refactor**: Refatora o código (melhoria sem alterar a funcionalidade).
* **test**: Adiciona ou modifica testes.
* **chore**: Realiza tarefas de manutenção (atualização de dependências, etc.).
* **build**: Modifica arquivos de build e dependências
* **ci**: Modifica arquivos e scripts de integração contínua.
* **perf**: Melhorias de performance.

## Exemplos

* `feat: adicionar funcionalidade de login`
* `fix: corrigir erro de validação no formulário`
* `docs: atualizar README com instruções de instalação`
* `style: formatar código de acordo com as diretrizes do projeto`
* `refactor: extrair lógica de autenticação para um módulo separado`
* `test: adicionar testes unitários para a função de login`
* `chore: atualizar dependências do projeto`

## Benefícios

* **Histórico claro**: Facilita a compreensão das mudanças ao longo do tempo.
* **Colaboração eficiente**: Permite que os membros da equipe entendam rapidamente as alterações.
* **Manutenção facilitada**: Simplifica a identificação e a correção de bugs.
* **Geração de changelogs**: Permite a criação automatizada de registros de alterações.

## Ferramentas

Existem ferramentas que podem auxiliar na padronização de commits, como:

* **Commitlint**: Verifica se as mensagens de commit seguem um padrão definido.
* **Husky**: Permite a criação de hooks Git para executar scripts antes de cada commit.
* **Commitizen**: Fornece uma interface interativa para criar commits seguindo um padrão.

A adoção de uma padronização de commits é uma prática fundamental para o desenvolvimento de software colaborativo e de alta qualidade.


