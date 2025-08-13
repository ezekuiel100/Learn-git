# Comandos principais do Git

## Iniciando e clonando repositórios

* `git init` — Inicia um novo repositório Git na pasta atual.
* `git clone <url>` — Clona um repositório remoto para o seu computador.

## Preparando arquivos para commit

* `git add <arquivo/pasta>` — Adiciona um arquivo ou pasta à área de *staging*.
* `git add .` — Adiciona todas as mudanças da pasta atual.
* `git status` — Mostra quais arquivos foram modificados ou adicionados.

## Criando e atualizando commits

* `git commit -m "mensagem"` — Cria um commit com os arquivos na área de staging.
* `git commit --amend -m "nova mensagem"` — Altera o commit mais recente.

## Branches

* `git branch` — Lista todas as branches e indica a atual.
* `git branch <nome>` — Cria uma nova branch.
* `git checkout <nomeDaBranch>` — Troca para outra branch.
* `git checkout -b <nome>` — Cria e muda para a nova branch.

## Histórico

* `git log` — Mostra o histórico de commits da branch atual.
* `git log --all` — Mostra todos os commits de todas as branches.
* `git log --all --graph --oneline` — Mostra o histórico de forma visual e resumida.

## Voltando mudanças

* `git reset` — Volta para um commit anterior.

  * `git reset --soft <commit>` — Mantém as alterações no *staging*.
  * `git reset --mixed <commit>` (padrão) — Remove do *staging*, mas mantém as alterações no diretório.
  * `git reset --hard <commit>` — Apaga todas as alterações após o commit (**irreversível**).

## Outros comandos úteis

* `git diff` — Mostra as mudanças feitas no código.
* `git stash` — Guarda temporariamente as mudanças não commitadas.
* `git pull` — Baixa as mudanças do repositório remoto.
* `git push` — Envia commits para o repositório remoto.
* `git merge <branch>` — Mescla uma branch na branch atual.
