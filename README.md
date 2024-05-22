# AprendendoGit

## 1. Configuração Inicial

### Instalação do Git
- Baixe o Git no [site oficial](https://git-scm.com/).
- Siga as instruções de instalação conforme o seu sistema operacional (Windows, macOS, Linux).

### Configuração inicial do Git (configuração de usuário, email)
- Configure seu nome de usuário:
  bash
  git config --global user.name "Seu Nome"
  
- Configure seu email:
  bash
  git config --global user.email "seuemail@example.com"
  

## 2. Repositórios Git: Local e Remoto

### Inicialização de um novo repositório
- Crie um novo repositório em um diretório existente:
  bash
  git init
  

### Clonagem de um repositório existente
- Clone um repositório remoto:
  bash
  git clone https://github.com/usuario/repositorio.git
  

### Diferença entre repositórios locais e remotos
- *Repositório Local:* Armazenado no seu computador, permite commits e histórico de versões.
- *Repositório Remoto:* Armazenado em um servidor (como GitHub, GitLab), permite colaboração e backup.

## 3. Trabalhando com Múltiplos Branches

### Criação e gerenciamento de branches
- Crie um novo branch:
  bash
  git branch nome-do-branch
  
- Mude para o branch criado:
  bash
  git checkout nome-do-branch
  

### Uso prático de branches para diferentes ambientes (desenvolvimento, produção)
- *Branch main ou master:* normalmente usado para produção.
- *Branch develop:* usado para desenvolvimento contínuo.

### Navegação entre branches
- Liste todos os branches:
  bash
  git branch
  
- Mude para outro branch:
  bash
  git checkout nome-do-branch
  

## 4. Integração com IDEs

### VSCode
- *Instalação da extensão Git:*
  - Pesquise por "Git" na seção de extensões do VSCode e instale.
- *Gerenciamento de branches e commits através do VSCode:*
  - Use a aba "Source Control" para visualizar alterações, fazer commits e gerenciar branches.

### Eclipse
- *Configuração do plugin EGit:*
  - Instale o EGit através do Eclipse Marketplace.
- *Execução de operações Git dentro do Eclipse:*
  - Use a perspectiva "Git Repositories" para gerenciar repositórios.

### Android Studio
- *Uso do controle de versão integrado para gerenciar projetos Android:*
  - Acesse VCS > Enable Version Control Integration e selecione Git.

## 5. Estratégias de Branching

### Estratégia de manutenção e produção separadas
- Manter branches diferentes para produção (main/master) e desenvolvimento (develop).

### Branches de feature: gerenciamento e melhores práticas
- Crie branches para cada nova funcionalidade:
  bash
  git checkout -b feature/nome-da-feature
  

## 6. Commits e Gerenciamento de Versão

### Realização de commits intermediários em desenvolvimento
- Faça commits frequentes para salvar progresso:
  bash
  git add .
  git commit -m "Descrição do que foi feito"
  

### Estratégias para commits limpos e eficazes
- Escreva mensagens de commit claras e detalhadas.

### Tagging para marcar lançamentos de versões
- Crie uma tag para uma nova versão:
  bash
  git tag -a v1.0 -m "Descrição da versão 1.0"
  
- Envie as tags para o repositório remoto:
  bash
  git push origin --tags
  

## 7. Fluxo de Trabalho Avançado

### BACKLOG
- Use ferramentas como Jira ou Trello para gerenciar backlog de tarefas.

### CHANGELOG
- Mantenha um arquivo CHANGELOG.md atualizado com as mudanças feitas em cada versão.

### VERSIONAMENTO EM 3 NÍVEIS (X.Y.Z)
- *Major (X):* Mudanças incompatíveis.
- *Minor (Y):* Novas funcionalidades compatíveis.
- *Patch (Z):* Correções de bugs.

## 8. Resolução de Conflitos

### Técnicas e ferramentas para resolução de conflitos
- Utilize ferramentas como git mergetool ou IDEs para resolver conflitos.
- Edite os arquivos em conflito e marque como resolvido:
  bash
  git add arquivo-resolvido
  git commit
  

## 9. Estudos de Caso e Melhores Práticas

### Exemplos reais de utilização do Git em projetos de software
- Projetos de código aberto no GitHub e GitLab.
- Utilização de Git em grandes empresas para gerenciamento de código.

### Dicas para manter a integridade do repositório
- Faça revisões de código antes de merges.
- Use CI/CD para testes automatizados antes de deploy.
- Mantenha o repositório limpo e organizado, removendo branches antigos e não utilizados.
