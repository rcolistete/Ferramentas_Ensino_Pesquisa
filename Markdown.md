# Markdown

Autoria : [Roberto Colistete Júnior](https://github.com/rcolistete).

Última atualização : 18/02/2021.

## O que é ?

[Markdown](https://en.wikipedia.org/wiki/Markdown) é uma linguagem simples para formatação de texto, permitindo títulos, negrito/itálico, listas, tabelas, links, imagens (locais e via link), citações de texto, citações de código-fonte, etc. É usada em Jupyter Notebook, editores de programação, em muitos sites/blogs em seção de comentários de matérias, em GitHub/GitLab/etc, etc. 

Por exemplo, este texto é escrito em Markdown, sem usar todos os recursos do mesmo, tendo sido usado o editor Typora (citado abaixo).

Há também variantes/flavours de Markdown. Uma das variantes/flavours é o Markdown do GitHub, sendo que é padrão em cada repositório (e até diretório) do GitHub ter um arquivo "README.md", onde ".md" é a extensão para arquivo MarkDown. Outros arquivos .md podem ser criados com outros nomes.

## Tutoriais sobre Markdown

Tutoriais diversos sobre MarkDown, em português :

- [Aprenda Markdown - DA2K blog](https://blog.da2k.com.br/2015/02/08/aprenda-markdown/);
- [Criando anotações com Markdown - alura](https://www.alura.com.br/artigos/criando-anotacoes-com-markdown);
- [Tutorial Markdown para iniciantes - Prof. Juliano Ramos blog](http://profjulianoramos.com.br/blog/markdown/2020/06/11/aprendamarkdown.html).

Em inglês :

- [Markdown-Cheatsheet - adam-p](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet);
- [Getting Started with Markdown - Sarah Simpkin](https://programminghistorian.org/en/lessons/getting-started-with-markdown);
- [Markdown Tutorial, com várias lições interativas](http://markdowntutorial.com/);
- [Tutorial ommonmark, com várias lições interativas](https://commonmark.org/help/tutorial/).

Do GitHub :

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/  
  );
- [Basic writing and formatting syntax](https://help.github.com/en/articles/basic-writing-and-formatting-syntax).

Do GitLab :

- [GitLab Markdown](https://docs.gitlab.com/ee/user/markdown.html);
- [Markdown Style Guide for about.GitLab.com](https://about.gitlab.com/handbook/markdown-guide/).

## Exemplos

Aqui uns exemplos de repositórios GitHub com "README.md" bem ricos, escolhi sobre MicroPython, do Peter Hinch :

- [micropython-lcd160cr-gui - A touch GUI for the official MicroPython display](https://github.com/peterhinch/micropython-lcd160cr-gui);
- [micropython-epaper](https://github.com/peterhinch/micropython-epaper);
- [Minimising Pyboard system power consumption](https://github.com/peterhinch/micropython-micropower/blob/master/HARDWARE.md).

Ou seja, quase toda a documentação de vários projetos pode ser feita em Markdown.

## Markdown x Jupyter Notebook x LaTeX

Eu recomendo :
- formato Markdown para escrever (evitando .doc, .txt, etc) textos de complexidade pequena a média em termos de formatação, pois é editável e visualizável em GitHub/GitLab, é formato leve, aberto/gratuito, tem editores diversos, inclusive para mobile OS (Android, iOS, etc);

- se o texto tiver mais complexidade, aí recomendo usar formato [Jupyter Notebook](https://jupyter.org/), que é também visualizável em GitHub/GitLab. Tal formato inclui MarkDown, além de MathJax/LaTeX (para expressões matemáticas), gráficos embutidos, código-fonte vivo (Python e outras dezenas de linguagens de programação) com resultados, etc;

- [LaTeX](https://www.latex-project.org/) para textos maiores mais complexos, com índice, capítulos/seções, bibliografia, etc. Por exemplo, para artigos, monografias, dissertações, livros, etc.

Curiosidade : dá para converter Markdown/Jupyter Notebook p/ LaTeX via [pandoc](https://pandoc.org/).

## Editores Markdown online

Markdown (editor) online permite testar e visualizar código/resultado em Markdown, muito prático. Tem muitos, alguns são editores com muitos recursos :

- [StackEdit](https://stackedit.io/);
- [Editor.md](https://pandao.github.io/editor.md/en.html);
- [Markdown Editor - jbt](http://jbt.github.io/markdown-editor/);
- [Markdown Live Preview](https://markdownlivepreview.com/);
- [Dillinger](https://dillinger.io/).

## Editores Markdown offline

A [lista de editores offline Markdown é gigantesca](https://letmegooglethat.com/?q=best+markdown+editors), segue aqui uma pequena seleção baseada em minhas preferências.

### Para Linux, Mac OS e Windows

#### Typora

Minha preferência.

<img src="https://typora.io/img/new/toc.png" alt="Typora" width="600"/>

[Typora](https://typora.io/) é um excelente software editor Markdown, permitindo editar enquanto visualiza o texto formatado (livre preview), com visual limpo mas cheio de recursos (inclusive uso de [expressões matemáticas com MathJax/LaTeX](https://support.typora.io/Math/), [diagramas](https://support.typora.io/Draw-Diagrams-With-Markdown/), etc), note que esses últimos recursos não são compatíveis com formato Markdown usual. É gratuito porém de código-fonte fechado, para Linux, Mac OS e Windows. Tem boa [documentação](https://support.typora.io/).  
Sugestão, decore os atalhos de teclado mais úteis :  Ctrl+K para inserir link no texto selecionado, Ctrl+/ para alternar modo código-fonte, etc.  
No Manjaro Linux, está disponível em [repositório AUR](https://aur.archlinux.org/packages/typora/) (da comunidade). 

#### ghostwriter

<img src="https://wereturtle.github.io/ghostwriter/images/html-preview.png" alt="ghostwriter" width="600"/>

[ghostwriter](https://wereturtle.github.io/ghostwriter/) é um editor Markdown razoável em recursos, com visualização lado-a-lado do texto formatado, gratuito e de [código-fonte aberto](https://github.com/wereturtle/ghostwriter), para Linux e Windows. Tem boa [documentação](https://wereturtle.github.io/ghostwriter/quickrefguide.html).  
Está disponível em repositórios Linux, como [Debian](https://packages.debian.org/search?suite=default&section=all&arch=any&searchon=names&keywords=ghostwriter) e [Arch/Manjaro](https://archlinux.org/packages/community/x86_64/ghostwriter/).

#### ReText

<img src="https://raw.githubusercontent.com/retext-project/retext/master/data/retext-kde5.png" alt="ReText" width="600"/>

[ReText](https://github.com/retext-project/retext) é um editor simples de Markdown, com visualização lado-a-lado do texto formatado, gratuito e de [código-fonte aberto](https://github.com/retext-project/retext), para Linux, Mac OS e Windows. Tem boa [documentação](https://github.com/retext-project/retext/wiki).  
Está disponível em repositórios Linux, como [Debian](https://packages.debian.org/search?keywords=retext) e [Arch/Manjaro](https://archlinux.org/packages/community/any/retext/).

### Joplin

<img src="https://joplinapp.org/images/DemoDesktop.png" alt="Joplin desktop" width="600"/>

[Joplin](https://joplinapp.org/) é um software para anotações, lista de tarefas, etc, que usa formato Markdown, com sincronização para os serviços de nuvem Nextcloud, Dropbox, OneDrive e WebDAV. É gratuito e multiplataforma [(Linux, Mac OS, Windows](https://joplinapp.org/#desktop-applications), [Android e iOS](https://joplinapp.org/#mobile-applications)), com [código-fonte aberto](https://github.com/laurent22/joplin).  
No Manjaro/Arch, está disponível em [repositório AUR](https://aur.archlinux.org/packages/joplin-desktop/) (da comunidade).

#### novelWriter

<img src="https://novelwriter.io/images/screenshot-multi.png" alt="Joplin desktop" width="600"/>

O editor Markdown [novelWriter](https://novelwriter.io/) é optimizado para textos mais longos com capítulos distribuídos em diferentes arquivos, etc. Tem [download gratuito e disponível para Linux, MacOS e Windows](https://novelwriter.io/download/), [código-fonte aberto](https://github.com/vkbo/novelWriter) e boa [documentação](https://novelwriter.readthedocs.io/en/stable/).  
No Manjaro/Arch, está disponível em [repositório AUR](https://aur.archlinux.org/packages/novelwriter/) (da comunidade). 

### Para mobile OS (Android, iOS, Sailfish OS, etc)

Tem muitos editores Markdown offline para mobile OS : [Android iOS](https://www.maketecheasier.com/markdown-editors-android/), [iOS](https://thesweetsetup.com/apps/our-favorite-markdown-writing-app-for-the-iphone/), [Sailfish OS](https://openrepos.net/search/node/markdown), etc. Meus preferidos são :
- "Markor" para Android, com download [via F-Droid](https://f-droid.org/packages/net.gsantner.markor/) ou [Google Play Store](https://play.google.com/store/apps/details?id=net.gsantner.markor&hl=pt_BR&gl=US), é gratuito e de [código-fonte aberto](https://github.com/gsantner/markor);
- Notizen.md para Sailfish OS, via [OpenRepos](https://openrepos.net/content/fooxl/notizenmd), é gratuito e de [código-fonte aberto](https://github.com/fuchsmich/notizenmd).

Muita gente usa editor (sem saber que é no formato Markdown) em smartphone para fazer anotações, desde lista de compras de supermercado, lista de tarefas, etc.é gratuitoé gratuito
