## exercicio01
Repositório para as aulas de CI/CD - Impacta
Modificação do Readme 

O Git é a ferramenta mais popular do SCM


--------------------------------


Iniciando com o GIT

-------------------------------


Passos - Atividade 1 
echo 02 > arquivo.txt 

 git commit -m "git add example -arquivo.txt"
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
  (commit or discard the untracked or modified content in submodules)    
        modified:   arquivo.txt
        modified:   aula02 (modified content)

no changes added to commit (use "git add" and/or "git commit -a")     

$ git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
  (commit or discard the untracked or modified content in submodules)    
        modified:   arquivo.txt
        modified:   aula02 (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

echo 02 > arquivo.txt


git diff:

$ git diff 
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'arquivo.txt', LF will be replaced by CRLF the next time Git touches it
diff --git a/.gitignore b/.gitignore
index 2211df6..8b13789 100644
--- a/.gitignore
+++ b/.gitignore
@@ -1 +1 @@
-*.txt
+
diff --git a/aula02 b/aula02
--- a/aula02
+++ b/aula02
@@ -1 +1 @@
-Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4
+Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4-dirty  


 git add . 
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'arquivo.txt', LF will be replaced by CRLF the next time Git touches it

git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   .gitignore

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
  (commit or discard the untracked or modified content in submodules)    
        modified:   aula02 (modified content)


git diff
diff --git a/aula02 b/aula02
--- a/aula02
+++ b/aula02
@@ -1 +1 @@
-Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4
+Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4-dirty 


echo 03 > arquivo.txt

git diff
warning: in the working copy of 'arquivo.txt', LF will be replaced by CRLF the next time Git touches it
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
diff --git a/aula02 b/aula02
--- a/aula02
+++ b/aula02
@@ -1 +1 @@
-Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4
+Subproject commit 570c69b1d9730a35b17f050cef3490caf85689f4-dirty  

$ git restore --staged arquivo.txt 

git commit -m "finalizando"
[main afaa122] finalizando
 1 file changed, 1 insertion(+), 1 deletion(-)

 echo *.txt > .gitignore 


 $ echo 04 > arquivo2.txt 

 git status 
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
  (commit or discard the untracked or modified content in submodules)    
        modified:   .gitignore
        modified:   arquivo.txt
        modified:   arquivo2.txt
        modified:   aula02 (modified content)



    git add .

    $ git commit -m "finalizando"
[main 1b8744f] finalizando
 3 files changed, 3 insertions(+), 3 deletions(-)

 git push 






