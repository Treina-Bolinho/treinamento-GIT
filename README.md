# Treinamento GIT, gitwork, e boas praticas
## 1. Descrição:

O objetivo desse treinamento é fazer o participante entender o funcionamento 
do git workflow que será usado em nosso projeto.

Esse repositório tem possui referências para outros materiais que devem ser 
consultados para que o treinamento seja efetivo.

O objetivo final é que o participante utilize as boas práticas do uso do git 
para trabalhar em conjunto com a equipe.

## 2. Primeiro passo

O primeiro passo para aprender a usar o [git workflow](https://nvie.com/posts/a-successful-git-branching-model/) é aprender a usar o git.

Segue uma lista de vídeos, cursos e blogs que irão te ajudar a entender o git:
* [Tutorial GIT da disciplina MDS](https://github.com/fga-eps-mds/A-Disciplina/wiki/Git)

* [Livro de GIT - Casa do Código](https://github.com/TosiGui/Fluxos-de-Trabalho/raw/master/Controlando%20vers%C3%B5es%20com%20Git%20e%20GitHub%20-%20Casa%20do%20Codigo.pdf)

* [Curso Git e Github para iniciantes - Udemy](https://www.udemy.com/course/git-e-github-para-iniciantes/)

* [Curso Learn Git - Codecademy](https://www.codecademy.com/learn/learn-git)

* [Curso de Git para iniciantes](https://www.youtube.com/watch?v=WVLhm1AMeYE&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
* [Como usar Git e Github na prática](https://www.youtube.com/watch?v=2alg7MQ6_sI)
* [Git Tutorial for Beginners](https://www.youtube.com/watch?v=HVsySz-h9r4)

### Objetivo 

Você estará preparado para aprender o git workflow quando você já se sentir 
confortável para:

* Clonar repositórios de remotos
* Criar branchs
* Adicionar arquivos novos na staging area do git
* Criar commits 
* Realizar merge entre branchs
* Deletar branchs
* Enviar alterações para repositórios remotos

## 3. Git workflow

O git workflow é um conjunto de práticas desenvolvido pelo [Vincent Driessen](https://nvie.com/posts/a-successful-git-branching-model/) que visa uma melhor organização em projetos que envolve várias pessoas.

O texto abaixo é um resumo grosseiro de diversos textos e vídeos assistidos. É altamente recomendado que você procure outras referenciais para entender o funcionamento do git workflow!

### 3.1. **Resumão**

Cada branch possui uma série de regras que devem ser respeitadas. Essas regras são:

Durante toda a vida do projeto somente 2 branch irão existir continuamente, a branch **master** e a branch **develop**.

A branch **master** somente irá aceitar códigos estáveis, onde já foi testado e corrigido erros e falhas. Somente 2 branchs podem realizar merge com a branch master, a branch **release** e a branch **hotfixes**

A branch **hotfixes** é utilizada quando é descoberto um erro grave no software que deve ser corrigido imediatamente, ou seja, foge do ciclo padrão de desenvolvimento. Assim é criado um branch a partir da **master** para devidas correções. Quando terminadas essa brach deve realizar merge com a branch **master** e com a branch **develop**. No final, essa branch é deletada.

A branch **develop** irá surgir a partir da master. Essa branch tem como finalidade reunir todas as features que serão desenvolvidas durante o ciclo de desenvolvimento do software. Ou seja, toda nova feature irá surgir a partir da **develop** e irá realizar merge com a **develop**.

Quando a branch **develop** agregar um conjunto de **features** satisfatório para entrega do software, irá surgir uma nova feature chamada **release**. 

Todo feature que for requisitada no projeto será desenvolvida em uma branch chamada **feature/{id-feature}-{nome-feature}**, esse padrão de nome serve para que os demais desenvolvedores saibam o que está sendo realizado nessa branch. Essa branch surgi a partir da branch **develop** e quando concluida as implementações é realizado o merge com a branch **develop**.

A função da branch **release** é testar o novo código desenvolvido e corrigir eventuais falhas e erros que podem surgir. Quando todos os erros e falhas estiverem corrigidos, essa branch irá realizar um merge com a **master**. No final essa branch é deletada.

Segue uma lista de vídeos, cursos e blogs que irão te ajudar a entender o git workflow:

* [Imagem da relação das branchs](https://i1.wp.com/lanziani.com/slides/gitflow/images/gitflow_1.png)

* [Texto original do criador do git workflow](https://nvie.com/posts/a-successful-git-branching-model/)

* [Texto em portugues sobre o git workflow - Mikael Hadler](https://medium.com/trainingcenter/utilizando-o-fluxo-git-flow-e63d5e0d5e04)

* [Texto em portugues sobre o git workflow - WILLIAN CAMPIDELI](https://imasters.com.br/desenvolvimento/quatro-workflows-para-trabalhar-com-git-melhores-2013)

* [Git flow na prática - Vídeo](https://www.youtube.com/watch?v=p1VAghNq-qg)

* [Workflow: Git - The Coding Train](https://www.youtube.com/watch?v=_sLgRBrZh6o)

* [GIT Workflow - Georgia Tech - Software Development Process](https://www.youtube.com/watch?v=3a2x1iJFJWc)

* [Git-flow Applied to a Real Project](https://medium.com/empathyco/git-flow-applied-to-a-real-project-c08037e28f88)

## Política de commits

As mensagens dos commits devem representar as modificações que foram realizadas. Assim foi criado uma padronização que se resume nos seguintes tópicos:

* A mensagem deve começar com #{id}, sendo id o número de identificação da issue em questão
* As mensagens devem ser escritas em ingles
* Os verbos devem está no imperativo, ou seja, não use added e sim add.

## Critérios de avaliação

Esse treinamento depende dos demais treinamentos. Será avaliado se você utilizou os conhecimentos obtidos nos demais projetos.

Tópicos de avaliação
* Utilização das branchs do git workflow
* Utilização da [política de commits](https://fga-eps-mds.github.io/2019.2-TimeBolinho/#/policies?id=commit-policies)

## Observações

Qualquer dúvida sobre os projetos entre em contato com o grupo
