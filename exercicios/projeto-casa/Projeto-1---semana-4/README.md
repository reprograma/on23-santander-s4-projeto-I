<h1 align="center">
  <img src="assets/reprograma-fundos-claros.png" alt="logo reprograma" width="500">
</h1>

# Tema da Aula

Turma Online 23 - Todas em Tech  | Front-end | Semana 4 | 2022 | Professora Thiele Nunes 
(Material construido a partir do material da prof Jaqueline)

Hoje é dia de revisão para assentar tudo o que você aprendeu até aqui.


### Instruções
Antes de começar, vamos organizar nosso setup.
* Fork esse repositório 
* Clique no botão "code"
* Copie o endereço do repositório
* Abra o seu Gitbash

* Entre no seu desktop:
```
     cd desktop
```
* Clone o fork na sua máquina: basta abrir o seu terminal e digitar:
  
```
     git clone url-do-seu-repositorio-forkado
```
* Digite o comando  ls para encontrar o seu repositório:
  
```
     ls
```
* Copie o nome do repositorio e entre na pasta clonada:
  
```
     cd on23-tet-s2-html-css
```
* Crie uma branch com o seu nome:
  
```
     git checkout -b seu-nome
```
* Digite o comando para abrir o projeto no vscode:
  
```
     code .
```

### Resumo
O que veremos na aula de hoje?
* [Revisão geral](#revisao)
* [HTML](#html)
* [CSS](#css)
* [Responsividade](#responsividade)
* * [Intervalos: Vamos comer  😋 e beber café! ☕](#intervalos)

     Vamos ter  dois intervalos : 10:30 e 15:00;

     Vamos almoçar às 12:00;

     Voltamos às 13:00.

## Conteúdo

### Revisão Geral
1. [O que vimos até agora?](#topico1)


### HTML
1. [Estruturas básicas](#topico3)
2. [HTML Semântico](#topico3)
3. [Class e ID](#topico3)

   
### CSS
1. [Link Style sheet](#topico4)
2. [USo de seletores](#topico4)
3. [Propriedades e valores](#topico4)

### Responsividade
1. [Mobile First](#topico4)
2. [Media Query](#topico4)
3. [Breakpoint](#topico4)

### Revisão 

#### O que vimos até agora

Vocês foram apresentadas ao HTML, CSS e Responsividade:

* Criaram uma página com estrutura básica;
* Conheceram as principais tags;
* Usaram HTML Semântico;
* Aprenderam a usar class e id;
* Descobriram como criar uma estilização para uma página;
* Estilizaram com tag, class e id.
* Mudaram a fonte;
* Aprenderam sobre unidades de medidas;
* Descobriram a importância de usar imagem com bosa resolução;
* Descobriram o media query e os breakipoint;
* Fizeram uma página responsiva.

**Ufa! Muita coisa, né?** 🙃

Mas o aprendizado é aos poucos. Vocês aprenderam os fundamentos e, a partir de agora o aprendizado estará em outro nível.

Continue e mantenha o foco em aprender um pouco a cada dia. 

### HTML

#### Estrutura básica
* [Principais Tags](#subtopico1)
* [HTML Semântico](#Subtopico2)

Com estes dois conceitos bem fixados, você vai longe!

##### Principais tags

- Tags estruturais: **html, meta,body, main, style, link,  title**
- Cabeçalho : **header, nav**
- Titulos: **h1 a h6**
- Parágrafo : **p**
- Link : **a e seus atributos**
- Listas: **ol, ul e li**
- Imagem: **img**
- Formulários: **form, input, label, textarea, fieldset**
- Formulários: **p** **table, th, td, tr**
- Rodapé:  **footer**
- Outras: **div, section, br**
  

##### HTML Semântico
O HTML semântico foi criado com o intuito de aproximar a linguaguem do HTMl da linguagem comum, usual, facilitando a leitura da desenvolvedora, auxiliando na indexação da página pelo Google, além de melhorar a acessibilidade no uso de leitores de tela.

* nav
* main
* article
* header
* aside
* footer
* section

#### Class e ID

As tags podem ser nomeadas de acordo com o conteúdo da página que está sendo criada para facilitar a estilização e possibilitar que uma tags com o mesmo nome possam ter estilos diferentes no css.

Para chamá-los, o padrão é:

```
  <p class="paragrafo"> Ola </p>

```
```
  <header>
  <p> Ola </p>
  </header>

```

Com o método **BEM** os nomes das classes e seletores seguem um padrão diferencia aquilo que é um conteúdo de bloco **B**, elemento **E** e modificadores **M**.
Utilizar o BEM é benefíco, rsss! 😅

### CSS

#### Link stylesheet

Para que a página tenha a sua estilização incluir a **tag style* dentro da *tag head*.
Há outras formas de chamar a taga style, mas a forma mais indicada é seguida abaixo:

```
    <link rel="stylesheet" href="style.css">

```

Criando um arquivo com extensão **css**, este arquivo é linkado conforme exemplo acima. Confira se o caminho incluido no **atributo href** está correto.

#### Uso de seletores

Para que seu conteúdo seja estilizado, é preciso chamar os seletores.
Os seletores são as tags e os nomes das class e id que você criou no html.

Exemplos:

```
    h1 {
      propriedade: valor;
    }

    h1, p{
      propriedade: valor;
    }

    .titulo {
      propriedade: valor;
    }

    .titulo__secundario {
      propriedade: valor;
    }

    footer > .titulo__rodape{
      propriedade: valor;
    }

    #article {
      propriedade: valor;
    }

```
#### Propriedades e valores

O CSS tem propriedades específicas para a estilização de cada tag/elemento. Nestas propriedades se encontram diversos valores utilizados de maneira generalizada e outros específicos.

```
   h1 {
      font-style: italic;
    }

   img {
    width: 100%;
   }

   p {
    font-size: 1.5em;
   }

```

Lembrando que o HTML já tem padrões para as tags e, quando utilizamos a estilização, mudamos estes padrões.
CSS é estudo, erro, estudo, acerto e erro de novo.

![css](https://media.giphy.com/media/YFkpsHWCsNUUo/giphy.gif)

### Responsividade

O layout responsivo traz fluidez para as nossas páginas, possibilitando  o uso do mesmo layout  de acordo com o tamanho da tela.
: **celular, table, desktop, laptop e televisão*.

As alterações no CSS acontecem com  o uso da técnica **media query**. Nesta técnica incluimos os break points - os pontos de quebra dos tamanhos das telas. 

#### Mobile first

A responsividade tem o conceito  **mobile first**, que orienta a estilização da página primeiro para o formato mobile(celular). Isso facilita o acesso de diversos usuários que têm o celular como principal meio de acesso à internet.

#### Media query

Media Query é a técnica que indica ao CSS que a partir da inserção da informação **@media (largura em px)** o layout terá outro comportamento.
É importante deixar o conteúdo que seja importante e necessário para a compreensão do usuário.

#### Breakpoints

O break point é o ponto em que a "tela quebra". Ele indica que a partir de determinada largura haverá uma mudança no layout da página telas mobile, tablet, laptop ou desktop.
Há um padrão dos break point que são mais utilizados, devido os diversos tamanhos de telas.


##### O que tambem vimos:

- Box Model (tem videos sobre no class room)
- Formularios (tem videos sobre no class room e tambem tem o nosso repositorio)
- Git/ Github (tem videos sobre no class room e tambem tem o nosso repositorio)
- Versionamento de codigo (tem videos sobre no class room e tambem tem o nosso repositorio)
- Criacao de repositorios, fork, clone, commits (tem videos sobre no class room e tambem tem o nosso repositorio)
- Terminal (tem videos sobre no class room e tambem tem o nosso repositorio)

##### Nossos repositorios:

- [Git/GitHub](https://github.com/reprograma/on23-santander-s1-git-github)
- [HTML/CSS](https://github.com/reprograma/on23-santander-s2-html-css/blob/main/README.md)
- [Responsividade](https://github.com/reprograma/on23-santander-s3-html-css-responsivo)

##### Ver ver rapidinho?
* BEM
- [bem](https://desenvolvimentoparaweb.com/css/bem/)

* text-align
- [text-align](https://www.w3schools.com/cssref/pr_text_text-align.php)


Chegamos ao final! Este é uma revisão de base para você dá continuidade aos seus estudos,

  
##### O que vamos ver na aula extra de CSS:

- [Justfy-content](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)
- [flex-direction](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)
- [grid](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column)
- [position](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning)
- [Display](https://github.com/reprograma/html-css-basico)
- [Display](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

### VAMOS AO EXERCICIO PARA SEMANA, M DE MARAVILHOSA! Projeto 01

* [Exercicio para casa](https://github.com/reprograma/on20-tet-s4-projeto-1/tree/main/exercicios/para-casa)

### Material da aula 

### Links Úteis
- [Principais Tags HTML](https://www.codigofonte.com.br/artigos/principais-tags-de-html)
- [O que é HTML Semântico](https://ayltoninacio.com.br/blog/o-que-e-html-semantico)
- [Método BEM](https://en.bem.info/methodology/html/)
- [Propriedades CSS](https://www.alura.com.br/apostila-html-css-javascript/39CA-propriedades)
- [Breakpoints de maneira coerra](https://desenvolvimentoparaweb.com/css/css-breakpoints-maneira-correta/)



<p align="center">
Desenvolvido com :purple_heart:  
</p>

