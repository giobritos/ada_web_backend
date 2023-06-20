# Git e Versionamento

Notes: Feito por Giovana de Brito Silva.
Seção: Seção 1

## Lecture Notes

# 1. O que é Git?

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/116936001adc80646292e88da026728c4f3fe16f/Git_e_Versionamento/Imagens/Untitled.png)

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled1.png)

# 2. Instalando e configurando o Git

```bash
sudo apt install git
```

```bash
git --version
```

# 3. Repositório do Git

Trazer do Github para a máquina:

```bash
cd /home/giovana/Documentos/Projetos

git clone https://github.com/giobritos/Ada_WebBackEnd.git
```

Trazer da máquina para o Github:

```bash
git init
```

# 4. Gravando mudanças no repositório

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled2.png)

Após realizar mudanças em um documento dentro do repositório:

```bash
git status
```

Stagging:

```bash
git add README.md
```

# 5. Git diff, commit e rm

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled2.png)

Git diff:

```bash
git diff **--staged**
```

Commit:

```bash
git commit -m "add new title"
```

# 6. Git log e restore

Git log:

```bash
git log
q #para sair do git log
```

Git restore:

```bash
git restore README.md
```

```bash
git restore **--staged** README.md
```

# 7. Repositórios remotos

```bash
git remote
```

```bash
git push origin master
#ou
git push origin main
```

```bash
git pull
```

```bash
git fetch
git diff origin/main #avalia as diferenças dos arquivos
q #sai do git diff (windows)
git pull #quando tiver certeza do conteúdo que está vindo do repositório remoto
```

# 8. GitHub

**GitHub** - Plataforma de hospedagem de códigos. 

# 9. Git branch

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled3.png)

```bash
git branch testing
```

```bash
git log --oneline --decorate
q #para sair (windows)
```

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled4.png)

```bash
git checkout testing
```

Fazendo commit de um arquivo pela branch testing temos uma imagem parecida com essa:

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled5.png)

```bash
git checkout main
```

Voltando para a main e fazendo um novo commit temos uma imagem assim (dois fluxos de trabalho diferentes que podem ser unidos futuramente):

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled6.png)

# 10. Merging branches

```bash
git branch 
```

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled6.png)

Para mergear as duas branches é necessário estar na branch main:

```bash
git merge testing
```

![Untitled](https://github.com/giobritos/Ada_WebBackEnd/blob/a1173b78964527ad9a0d9954c09fad6b4cfbb79b/Git_e_Versionamento/Imagens/Untitled7.png)
