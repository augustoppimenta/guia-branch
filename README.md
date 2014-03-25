Aprendendo um pouco sobre Branch
==========

Bem, recentemente disponibilizei aqui no GitHub um [Guia para iniciantes](https://github.com/augustoppimenta/guia-git-github). Agora irei apresentar (superficialmente) os Branches, uma funcionalidade incrível do Git.

GIT
----------

Sempre o nosso primeiro passo é acessar a pasta da aplicação.

1. Acesse a pasta da aplicaçao:

```
$ cd <nome_do_diretorio>
```
Agora precisamos criar nosso primeiro Branch.

Observação: Este guia subentende que você já passou pelo Guia para iniciantes.

2. Dentro da pasta da aplicação digite o seguinte comando:

```
$ git branch testing
```
Pronto, criamos um branch chamado "testing".

3. Bem, agora vamos visualizar quais branch possuímos:

```
$ git branch
```

Com esse comando aparecerá uma listagem com todos os branches que seu projeto possui. Muito provavelmente a listagem será igual a esta abaixo:

```
*master
testing
```

Observação: O "*" aponta para o branch que seu projeto está localizado.



4. Bem, agora para mudarmos de branch precisamos fazer um simples comando:

```
git checkout testing
```

5. Se repetirmos o mesmo comando do "Passo 3", notaremos que a nossa aplicação está apontando para o branch "testing":

```
master
*testing
```

Feito isso, já podemos já podemos trabalhar em nossas melhorias. Daí surge uma pergunta: "Mas depois que eu concluir minhas melhorias, realizar meus commits e testá-las, posso juntar todo o trabalho no branch master? A resposta é? SIM!!!!!". Para tal, devemos fazer os seguintes procedimentos:

6. Retornar para o branch master

```
git checkout master
```

7. E realizar um "merge"

```
git merge testing
```

Fim! Tudo agora está agrupado.


8. Agora é só fazer o:

```
git commit -m "Projeto finalizado"
```

9. 
```
git push origin master
```

Novamente será solicitado seu login e senha do GitHub.

FIM!

Ajuda
----------
Se você quiser ajudar a melhorar este guia, escrevendo, corrigindo ou aprimorando a experiência, por favor, faça um FORK do projeto e mãos na massa.

Avançando
----------
Caso você esteja super ancioso para aprender mais e mais sobre o Git, recomendo a leitura do livro do [Git](http://git-scm.com/book/pt-br/), em português.

Caso queria praticar um pouco, recomendo o [TryGit](http://try.github.io/levels/1/challenges/1).

Abraço!

