# Comandos Essenciais do Git

Este arquivo lista e explica os principais comandos do Git, mostrando para que servem e como usá-los.

---

## 1. git init
Inicializa um novo repositório Git na pasta atual.

```bash
git init
````
2. git clone
Clona um repositório remoto para sua máquina local.

```bash

git clone https://github.com/usuario/repositorio.git

```
3. git status
Mostra o status dos arquivos do repositório: modificados, não rastreados ou prontos para commit.

```bash

git status
```
4. git add
Adiciona arquivos ao stage para o próximo commit.

```bash

git add nome-do-arquivo
git add .   # adiciona todos os arquivos modificados
```
5. git commit
Cria um commit com as alterações adicionadas ao stage.

```bash

git commit -m "mensagem do commit"
```
6. git push
Envia commits da branch local para o repositório remoto.

```bash

git push origin nome-da-branch

```
7. git pull
Atualiza sua branch local com as mudanças do repositório remoto.

```bash

git pull origin nome-da-branch
```
8. git branch
Lista, cria ou deleta branches.

```bash

git branch       # lista branches
git branch nova-branch  # cria branch
git branch -d branch-velha  # deleta branch
```
9. git merge
Une uma branch na branch atual.

```bash

git checkout main
git merge feature/alguma-coisa
```
10. git rebase
Aplica commits de uma branch em outra, reorganizando o histórico.

```bash

git checkout feature/alguma-coisa
git rebase main
```
11. git stash
Guarda temporariamente alterações não commitadas, para depois recuperá-las.

```bash

git stash       # guarda alterações
git stash apply # recupera alterações
```
