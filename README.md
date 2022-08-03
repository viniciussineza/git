# Git - Control Version

### 1. Criar um repositório no github.

### 2. Copiar a URL do repositório e abrir no GitPod

### 3. Criar um index.html

Commit == check-point

git status

```
On branch main

No commits yet

Untracked files:
    (use "git add...")
        index.html

nothing added to commit but untracked files
```

**Working directory** - Versão salva no seu HD
**Alterações não salvas não existem** !important

**Staging Area** - Cópia do working directory para uma área de espera

git add index.html 
(sem retorno no terminal)

git status

```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
```

Duas versões - Uma no working directory e uma no stage Area
Ao modificar o index.html

On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

Existe a notificação da modificação, por menor que seja

git add index.html 

git status

```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
```

git commit

Abre um editor no vscode ou o próprio editor do linux e só finaliza o commit após salvar e fechar o arquivo.

[main (root-commit) 6e97bf2] Commit inicial do projeto
 1 file changed, 12 insertions(+)
 create mode 100644 index.html

 git status

 On branch main
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

nothing to commit, working tree clean

git log

commit 6e97bf25789159dbb0f4f9b2552ac6a7405fbe4a (HEAD -> main)
Author: Vinicius Sineza <viniciussineza@gmail.com>
Date:   Tue Aug 2 23:01:05 2022 +0000

    Commit inicial do projeto
    
    Cria a página index.html com a saudação Hello World


git commit --ammend

git commint --help

git restore index.html
retorna para a última versão

git restore --staged index.html (Retorna do add)

git log --oneline (retorna os commits em uma linha)

git push (enviar remote)