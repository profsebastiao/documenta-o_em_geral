# 📘 Manual Básico de Git

Este guia fornece os comandos essenciais para começar a utilizar o **Git**, um dos sistemas de controle de versão mais utilizados no mundo.

---

## 🛠️ Instalação

### Linux (Debian/Ubuntu)
```bash
sudo apt update
sudo apt install git
```

### Windows e Mac
Baixe o instalador no site oficial:  
🔗 https://git-scm.com/downloads

---

## 🔧 Configuração Inicial

Configure seu nome e email (importante para os commits):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Verifique as configurações:

```bash
git config --list
```

---

## 📂 Criando ou Clonando um Repositório

### Criar um novo repositório
```bash
git init
```

### Clonar um repositório remoto
```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 🔄 Ciclo de Versionamento

### Verificar o status do repositório
```bash
git status
```

### Adicionar arquivos ao staging
```bash
git add nome_do_arquivo.ext
# ou tudo:
git add .
```

### Fazer um commit
```bash
git commit -m "Mensagem do commit"
```

### Ver histórico de commits
```bash
git log
```

---

## 🌐 Trabalhando com Repositórios Remotos

### Adicionar origem remota
```bash
git remote add origin https://github.com/usuario/repositorio.git
```

### Enviar alterações para o GitHub
```bash
git push -u origin main
```

> Substitua `main` por `master` se o repositório usar esse nome de branch.

### Baixar atualizações do repositório remoto
```bash
git pull origin main
```

---

## 🌿 Branches

### Criar uma nova branch
```bash
git checkout -b nova-branch
```

### Listar branches
```bash
git branch
```

### Alternar entre branches
```bash
git checkout nome-da-branch
```

### Mesclar uma branch com a principal
```bash
git checkout main
git merge nome-da-branch
```

---

## 🚫 Desfazendo Mudanças

### Remover arquivo do staging
```bash
git reset nome_do_arquivo.ext
```

### Voltar um commit (sem perder alterações locais)
```bash
git reset --soft HEAD~1
```

### Voltar um commit e apagar alterações
```bash
git reset --hard HEAD~1
```

---

## 🗃️ .gitignore

Crie um arquivo `.gitignore` para ignorar arquivos/pastas:

Exemplo:
```
node_modules/
.env
*.log
```

---

## 🧠 Dicas úteis

| Ação                         | Comando                        |
|-----------------------------|--------------------------------|
| Ver arquivos modificados    | `git status`                  |
| Ver diferença entre versões | `git diff`                    |
| Criar tag de versão         | `git tag -a v1.0 -m "v1.0"`   |
| Clonar com SSH              | `git@github.com:usuario/repo.git` |

---

## 📚 Recursos úteis

- 🔗 [Documentação oficial do Git](https://git-scm.com/doc)
- 🧠 [Git Cheatsheet (GitHub)](https://education.github.com/git-cheat-sheet-education.pdf)
- 📹 [Curso Git e GitHub - YouTube](https://www.youtube.com/results?search_query=git+e+github)

---

## 👤 Autor

**Sebastião Bastos**  
💻 Canal: Vivendo com tecnolgia  
🔗 [LinkedIn](https://www.linkedin.com/in/profsebastiao) | [GitHub](https://github.com/profsebastiao)
