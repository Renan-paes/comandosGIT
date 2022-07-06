
<p><img src="https://sujeitoprogramador.com/wp-content/uploads/2021/04/gitimage.png"></p>

# comandos GIT
### ✅ Se você está começando do zero, _vou te orientar desde a instalação do **Git** até o primeiro push_.

### ⚠️ _PS: esses comandos são baseados no meu entendimento. Qualquer dúvida, deixe-me uma mensagem_ ⚠️



<div style=background:#245fff;font-size:16px;padding:20px;border-radius:5px;margin-top:20px;>

1. Instalar o git.

2. Criar conta no github.

3. Crie uma pasta e execute a mesma com o gitbash.

4. Criar um arquivo de texto dentro da pasta.

5. Dentro do gitbash dar um "git status" para ver sua situação.

6. Dar um git add "nome do arquivo".

```
// Eu adicionei mais 2 arquivos e utilizei o  "git add ." para trackear todos ao mesmo tempo.
```

7. git commit -m "primeiro commit"

```
// Ele está pedindo para configurar o seu email e nome
// $ git config --global user.name "Fulano de Tal"
// $ git config --global user.email "fulanodetal@exemplo.br"
```

8. git commit -m "commit inicial"

9. git push // Ele não vai pegar por que você vai ter que criar um repositorio em seu github e só assim vai dar certo

10. git remote add origin https://github.com/Renan-paes/projeto1-Git

11. git push // Não vai dar certo, simplesmente copie o nome do push que vai aparecer no seu terminal

12. git push --set-upstream origin master (No meu apareceu esse)

13. Talves você precise fazer o login no github, autorize-o.
</div>

<h1 style=margin-top:80px;background:#F05032;border-radius:10px> 
<img width='40px'; src="https://user-images.githubusercontent.com/77288669/177601509-43aa1914-6be3-4ba2-b660-eec37349acd7.png"> Comandos para você usar no seu dia dia.</h1>

```git
.1 git --version // Para ver a versão do seu git
```
```
.2 git config --global user.name "seuNome" // Configura seu nome dentro do git *importante
```
```
.3 git config --global user.email "seuEmail" // Configura seu email dentro do git *importante.
```

```
.4 git config user.name OU git config user.email  // Verifica o status referente a cada um.
```
```
.5 git config --list  // Você consegue ver a configuração do seu git.
```
```
.6 git checkout -- nomeDoArquivo  // Você consegue resgatar o que era antes da modificação, como estava no diretório de trabalho
```
```
.7 git reset HEAD nomeDoArquivo     // Se você deu git add e quer tirar o arquivo da stage area.
```
```
.8 git reset -- soft (ex. 323554) (Nesse você só desfaz o commit e não perde os arquivos no diretorio de trabalho.
```
```
.9 git reset --hard (ex. 34fgtyd) (*PERIGO* Nesse caso você vai mudar o seu ponteiro HEAD para outro commit e apagar tudo que foi feito, bem diferente do SOFT.)
```

```
.10 git commit --amend     // Renomear o commit (aperta i para entrar no modo digitar, depois de corrigir aperte o ESC e escreva para sair,  :wq e ENTER )
```
```
.11 git commit --amend -m "Renomeando o último commit"  // Maneira mais fácil para renomear o ultimo commit
```
```
.12 git branch     // Você vê todas as branchs existentes e em qual você se encontra, porém é apenas localmente
```
```
.13 git branch -a     //  Você vê todas as branchs existentes e em qual você se encontra, ESSA É LOCAL E REMOTA
```
```
.14 git branch nomeDaBranch     // Você cria uma branch nova (Certifique de vê se você está na branch main para criar novaBranch a partir dela)
```
```
.15 git checkout -b novaBranch     // Você cria a branch e já fica dentro dela
```
```
.16 git checkout nomeDaBranch     // Troca para branch que deseja escolher
```
```
.17 git branch -m novoNome     // Você muda o nome da branch
```
```
.18 git branch -d nomeDaBranch     // Para deletar uma branch local (Tem que estar fora dela para deletá-la)
```
```
.19 git branch -D nomeDaBranch     // Se o primeiro não deletar coloque 'D'
```
```
.20 git remote -v   // Esse comando nos mostra o endereço do repositório remoto para o qual estamos enviando nossos códigos
```
```
.21 git push -u origin minha-branch  // CRIA branch REMOTA
```
```
.22 git push origin -d minha-branch   // DELETA branch REMOTA
```
```
.23 git push origin --delete nomeDaBranch     // Para deletar uma branch remota
```
```
.24 git merge nomeDaBranch     // Para puxar as informações de outra branch para a sua atual ( Quando você dá merge significa que a branch que você está atualmente vai receber o conteúdo da branch que você deseja receber, a tal 'nomeDaBranch'
```
```
.25 git stash     // Volta para o estágio inicial toda seu diretorio de trabalho, porém te dá um código para você reverter
```
```
.26 git stash push -m meu-novo-stash     // O mesmo de cima mas você coloca um nome na sua stash
```
```
.27 git stash list     // Você consegue ver a chave e ID para reverter
```
```
.28 git stash apply numeroDoID     // Você volta tudo como estava, ex: 0, 1,3,10 .. ficando dentro do {0}. As stash mais recentes ficam no inicio.
```
```
.29 git stash drop numeroDaStash     // DELETA a stash que deseja colocando o número dela. 
```
```
.30 git tag -a v1.0 -m "primeira versao do sistema"     // Criando tag ( Lembrando que você escreve a versao que deseja ex: v1.0)
```
```
.31 git tag     // Você consegue ver a versao da sua tag (V1.0 QUE CRIEI na anterior)
```
```
.32 git show tag     // Visualiza sobre a tag
```
```
.33 git checkout nomeDaTag     // Você visualiza como estava seu codigo naquela versão << Essa versão é melhor do que a git show
```
```
.34 git push origin versaoDaTag     // Aqui você envia para o github individualmente a tag escolhida
```
```
.35 git push origin --tags     // Aqui você envia todas as tags para o github
```
```
.36 git clone https://github.com/Renan-paes/github_Teste.git .     // Clonou um projeto e o 'ponto no final' foi para puxar apenas o conteúdo e não a pasta principal que envolve o conteúdo.
```
```
.37 git clone https://github.com/Renan-paes/github_Teste.git      // Clonou um projeto mas veio a pasta também
```
```
.38 git clone https://github.com/Renan-paes/github_Teste.git NomeDaPasta // Clonou e já colocou um novo nome na pasta principal
```
```
.39 git fetch -a     // Vai buscar no repositório para saber se tem alguma atualização no repositorio ( se der git checkout 'nomeDessaTalBranch' )
```
```
.40 git log     // Você visualizar o histórico de commit
```
```
.41 git log --oneline  // Você consegue visualizar os commits mais curto
```
```
.42 git log --oneline -5 // É o mesmo de cima mas só aparecerá os 5 primeiros 
```
```
.43 git shortlog   // Você apenas vê o nome dos commits e quem fez
```
```
.44 git log --author= nomeDaPessoa     // Mostra o histórico de commits feitos por uma única pessoa, excelente para saber que fez o quê.
```
```
.45 git reflog   // Você consegue visualizar cada modificação mais detalhada DENTRO DA SUA BRANCH incluindo quando você sai de uma branch e vai para outra
```
```
.46 git log --grep 'trechoDaMensagemDoCommit'   // Mostra o histórico de commits filtrado por uma mensagem.Caso você se lembra de um trecho do seu commit dá pra achar com esse comando.

também pode ser buscado como...
// procurar por "produtos" OU "usuarios"
$ git log --grep produtos --grep usuarios

// procurar por "produtos" E "usuarios"
$ git log --grep produtos --and --grep usuarios

```
```
.47 git log --all --decorate --oneline --graph   // imprimir o histórico exibindo as branches do repositório com algo mais legível e com cores com apenas esse comando.
```
```
.48 git remote add origin https://meu-endereco.com/meu-projeto.git   // Adicionar um repositorio remoto
```
```
.49 git blame -w -L 1,12 nome-do-arquivo  // Para saber quem fez cada linha de um ARQUIVO (Nesse aparece o nome da pessoa)
```
```
.50 git blame -w -L 1,12 nome-do-arquivo -e  // Mesmo caso de cima, porém aparece o email no lugar do nome
```
```
.51 git gc  // Otimiza o repositório
```
```
.52 git diff  // Você compara o seu repositorio local com o remoto
```
```
.53 git diff HEAD: nomeDoArquivo  // Nesse caso você vai fazer a comparação do repositorio local com o remoto de um arquivo específico
```
```
.54 notedpad nomeDoDocumento.js  // Você cria um arquivo pelo terminal. Pode ser  .txt .html .css
```
```
.55 git mv nomeDoArquivo  novoNomeDoArquivo  // Renomear um arquivo após ele estar sendo monitorado pelo git
```
```
.56 git show HEAD // Mostra as alterações do próprio documento, apenas dele.
```



<h1 style="margin: 50px auto">👨‍💻 Contribuidor </h2>
<table style="margin: 30px auto">
    <tr>
        <td><img style="border-radius:50%" src="https://user-images.githubusercontent.com/77288669/177606856-41f7b943-ee69-4a30-bfab-555a9397b41d.jpg"></td>
    </tr>
    <tr>
        <td style="font-size:25px">Renan Paes</td>
    </tr>
    <tr style="text-align:center; background:#00f">
        <td><a  href="https://www.linkedin.com/in/renan-paes-00ba02208/" target="_blank" rel="noopener noreferrer" >Linkedin</a></td>
    </tr>
    
</table>
