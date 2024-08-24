
# DIO | Git & GitHub

 Guia de Uso do Git e Git Bash

## Introdução
Este guia oferece uma visão geral sobre Git e Git Bash, incluindo comandos essenciais e práticas recomendadas para o uso eficiente dessas ferramentas.

## Conceitos Importantes

### Git: Controle de Versão Distribuído
Git é um sistema de controle de versão distribuído que permite rastrear alterações no código-fonte durante o desenvolvimento de software.

### GitHub: Repositórios Remotos
GitHub é uma plataforma baseada na web que hospeda repositórios Git e facilita a colaboração entre desenvolvedores.

### Branches Principais: `main` vs `master`
- **Main**: A branch principal moderna, adotada por muitas plataformas de hospedagem de repositórios.
- **Master**: A branch principal tradicional, usada historicamente como padrão.

## Git Bash: Uso do Terminal e Comandos Essenciais

### Navegação Básica
- `pwd`: Exibe o diretório atual.
- `cd <diretório>`: Navega entre diretórios.
- `ls`: Lista os arquivos e pastas no diretório atual.
- `mkdir <nome-do-diretório>`: Cria um novo diretório.
- `touch <nome-do-arquivo>`: Cria um novo arquivo vazio.
- `rm <nome-do-arquivo>`: Remove um arquivo.
- `rm -r <nome-do-diretório>`: Remove um diretório e todo o seu conteúdo.

### Configurações Iniciais
- `git config --global user.name "Seu Nome"`
- `git config --global user.email "seuemail@example.com"`
- `git config --list`

### Trabalhando com Repositórios
- `git init`: Inicializa um novo repositório GIT no diretório atual.
- `git clone <URL>`: Clona um repositório remoto.
- `git status`: Exibe o status atual do repositório.
- `git log`: Mostra o histórico de commits.
- `git diff`: Mostra as diferenças entre arquivos que ainda não foram commitados.

### Controle de Versão
- `git add <arquivo>`: Adiciona um arquivo à staging area.
- `git commit -m "Mensagem do Commit"`: Faz um commit das mudanças.
- `git push`: Envia commits locais para o repositório remoto.
- `git pull`: Integra mudanças do repositório remoto.
- `git branch`: Lista as branches.
- `git checkout <branch>`: Muda para a branch especificada.
- `git merge <branch>`: Mescla a branch especificada na branch atual.

### Atalhos e Dicas
- **Autocompletar**: Use `Tab` para autocompletar comandos e caminhos.
- **Histórico de Comandos**: Use `↑` e `↓` para navegar no histórico.
- **Limpar a Tela**: Use `Ctrl + L` para limpar o terminal.
- **Cancelar Comando**: Use `Ctrl + C` para interromper um comando.

## Solução de Problemas Comuns

### Erro: `destination path already exists and is not an empty directory`
Este erro ocorre ao tentar clonar um repositório em um diretório que já existe e não está vazio. Para resolver:
1. **Remover o Diretório Existente**:
   ```bash
   rm -rf <caminho-do-diretório>
   git clone <URL> <caminho-do-diretório>

