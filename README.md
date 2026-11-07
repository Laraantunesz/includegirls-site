
# Portal institucional do projeto de extensão include girls
## 🚀 Como Executar Localmente
Siga os passos abaixo para baixar o repositório na sua máquina e visualizar o site em desenvolvimento.

### 📋 Pré-requisitos

* [Git](https://git-scm.com/) instalado no computador.
* [Visual Studio Code](https://code.visualstudio.com/) (recomendado).
* Extensão **Live Server** instalada no VS Code (opcional, mas recomendada visualizar o site no decorrer do desenvolvimento).

---

### 1. Clonar o repositório

Abra o terminal (Git Bash no Windows ou terminal padrão no Linux/macOS), navegue até a pasta onde deseja guardar seus projetos e execute:

```bash
# Clone o repositório
git clone https://github.com/Laraantunesz/includegirls-site.git
```
## 📁 Estrutura de Diretórios e Arquivos

     📦 includegirls-site/
      ├── 📄.editorconfig         # Padroniza espaçamento, indentação e quebras de linha entre editores*
      ├── 📄.gitignore            # Impede o versionamento de arquivos locais desnecessários
      ├── 📄README.md             # Documentação geral e guia do projeto
      ├── index.html              # PÁGINA INICIAL (Home)
      ├──📁pages/                 # Diretório reservado para todas as páginas secundárias
      │   └──sobre.html            # Futura página sobre nós
      └──📁assets/                # Recursos estáticos compartilhados por todo o site
          ├── 📁css/
          │   ├── variables.css   # Tokens visuais (paleta de cores do projeto, fontes e medidas)
          │   └── style.css       # Folha de estilos principal e customizações do layout
          ├── 📁js/
          │   └── main.js          # Scripts gerais, inicialização de componentes e interações
          └── 📁img/              # Imagens, logotipos institucionais, fotos e ícones
## 📂O que vai em cada pasta

  - index.html (Raiz):
      Contém a estrutura global completa (Skip Links, Header gov.br, Menu principal, conteúdo da Home e Footer oficial).

  - pages/:
      Armazena exclusivamente as páginas internas e secundárias conforme forem desenvolvidas (ex.: sobre.html,equipe.html).


  - assets/:
    - assets/css/:

      - variables.css: centraliza as cores da identidade visual do projeto garantindo que alterações visuais reflitam em todas as telas.

      - style.css: reúne as regras de layout, alinhamentos, espaçamentos e ajustes complementares da aplicação.

    - assets/js/:

      - main.js: concentra a lógica de comportamento do portal, como controles de abertura/fechamento de menus responsivos, validações de acessibilidade e futuras integrações de bibliotecas.

    - assets/img/: Guarda todos os arquivos de mídia como logotipos,fotos de eventos, banners ou ícones

## ⚙️Controle de Versão com GitHub

 ### Bons hábitos de desenvolvimento:

  - Nunca faça commit e push direto na main. A branch main representa o código estável e pronto do projeto.

  - Antes de começar as alterações no código se certifique qeu está na versão mais atualizada da main e depois mude para a branch em que irá trabalhar:

    - Garanta que está na main e atualize-a

        ```bash
        git checkout main 

        git pull origin main
    - Crie ou mude para a sua branch:
        - Alternar para um branch que já existe: 
        ```bash
         git switch nome-da-branch
         ```
        - Criar nova branch e mudar automaticamente para ela: 
        ```bash
        git switch -c nome-da-nova-branch
### O que fazer antes do commit:

  - **Testar localmente no navegador**: Nunca envie código que não foi testado.
  - **Revisar o status e as alterações**:
    - Execute **git status** para confirmar quais arquivos foram modificados ou adicionados.
    - Se quiser verificar linha por linha execute **git diff**.

  - **Adicionar** os arquivos modificados:
    - **git add nome-arquivo** ou **git add .**

### Commit no padrão gov:

  - O próximo passo é fazer  commit: 
    ```bash
      git commit -m "mensagem"
    ```

  - Cada commit deve começar com um prefixo específico que indica a natureza da mudança.

  *Padrão dos commits:*

   - **feat**: Nova funcionalidade, página ou seção

  - **fix**: Correção de bug funcional ou erro de layout

  - **style**: Ajustes visuais, CSS ou indentação sem mexer na lógica

  - **docs**: Mudanças exclusivamente em documentação

  - **refactor**: Reorganização de código sem mudar a funcionalidade externa

  - **chore**: Atualizações de tarefas de build, configurações gerais ou pacotes que não modificam o código de produção.

*EX: git commit -m "feat: adicionar pagina Sobre nos"*

### Enviar alterações feitas para o repositório:

- Sincronizar com a branch principal:
  ```bash
  git pull origin main
- Enviar código local para o repositório:
  - Se for o primeiro envio da branch: 
  ```bash
  git push -u origin nome-da-sua-branch
  ```
  - Se já enviou algo anteriormente: 
  ```bash
    git push
  ````


- Todo código novo deve entrar na main exclusivamente por meio de Pull Requests (PR), isso garante a revisão de código antes de alterar a branch oficial.Passo a passo: 
    - Acesse a página do projeto no GitHub no navegador e vá para pull requests, depois new pull request. 
    - Configure os Branches no topo da página:
        - base: escolha a branch de destino (ex: main).
        - compare: escolha a sua branch com as alterações(ex: minha-nova-feature).
    - Preencha o título e a descrição do Pull Request e clique em Create pull request.   


