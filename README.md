# GIT
Lançado em 07/04/2005
lunux torval criador do git e linux

não confundir git com github

## GitHub
### O que é o GitHub?
É uma plataforma que utiliza o sistema GIT, permitindo que criemos o que chamamos de repositórios (onde podemos colocar nossos projetos e trabalhar de forma colaborativa com outros desenvolvedores no mesmo projeto).

## Registros de utilizador no GitHub
Criamos através do site https://github.com, tem conta free e pro.

## Instalação do GIT no sistema
Baixe a última versão diponível para seu sistema operacional no site https://git-scm.com/

Faça a instalação com as opções padrões, so mude o editor de texto para o vscode ou outro ao qual esteja usando

### configurando nome e email
git config --global user.name "{seu-nome}"
git config --global user.email "{seu-email}"

## Criação de repositório
Acesem sua conta GitHub no site https://github.com, se não tiverem nenhum projeto clique no botão `Start a project`, em `New` ou `New Repository`.

Será direcionado a https://github.com/new, então preencha as informações do seu repositório:
* Repository name;
* Description (optional);
* Public or Private;
* Initialize this repository with:
    * Add a README file: arquivo para descrever o projeto;
    * Add .gitignore: arquido do git utilizado para ignorar arquivos, pastas ou extensões no versionamento, ou seja, se adicionarmos *.tmp os;
    * Choose a license;

Então clique em `Create repository`

## Clonagem de repositório
copiamos o link do nosso repositório no git e clonamos na em uma pasta local onde desejar e no terminal executar:
```git
git clone https://github.com/{nome-da-sua-conta}/{nome-do-seu-repositorio}.git
```
Esse comando irá criar uma pasta com o nome do seu projeto dentro da pasta que voce rodar o `git clone`.

## Etapas de um desnvolvimento
Segue possiveis etapas do dia a dia de desenvolvimento:
git add .
git commit -m "sua-descrição"
git push

* **Alterações**: Adicionamos e/ou alteraramos os arquivos de desenvolvimento, configurações ou outro quaquer que faça parte do projeto;
* **Stage**: 
    * adicionamos todos arquivos a serem enviados ao repositório;
    * nesta etapa podemos listar os arquivo novos ou alterados com o `git status`;
    * e adicionamos todos ou apenas alguns:
        * para todos utilizamos o `git add .`, que setará todos arquivos novo e/ou alterados para serem comitados;
        * também podemos mandar um a um passando o nome ou caminho relativo se ele estiver em outra pasta:
            * `git add index.php`;
            * `git add ../index.php`;
            * `git add conf/lang.php`;
* **Commit**: Adicionamos uma descrição relevante do que estamos enviando ao repositório.
* **Push**: Agora vamos enviar as alterações ao repositório com o `git push`.

Neste momento podemos ter conflitos caso alguem tenha feito um commit antes e eu não tenha atualizado meu repositório local.

Caso o conflito seja em um arquivo que voce não tenha alterado, basta fazer o `git pull` e o `git push` na sequencia.

Já se o conflito for em um arquivo que também alteramos, então teremos que trata-lo, tente atualizando o repositório local com o `git pull`, resolva os conflitos e de apenas um `git commit`, assim ele passará para o `stage merge`, então tente o `git push` novamente, se não tiver outra alteração irá funcionar, caso contrário terá que resolver os conflitos.

## Preparar um projeto existe para funcionar com repositório GIT

## Utilização do GIT no desenvolvimento de um projeto

## Principais funcionalidades do GIT

https://www.youtube.com/watch?v=gitK9Qe1D0U&list=PLXik_5Br-zO_mAJllNIF5K_ujRgnrHinr&index=5



