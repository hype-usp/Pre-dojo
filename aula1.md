# Uma introdução à Python

Python é uma linguagem de programação de alto nível e uso geral, criada em 1991 por Guido Von Rossum, tendo como máxima ser uma linguagem simples de aprender, fácil de entender, e bastante expressiva em seu código. Ela virou a língua-mãe para projetos que precisam de uma prototipação rápida e que demande o menor número possível de mão de obra, exatamente pela sua simplicidade e eficiência.

Por prezar em ser uma linguagem fácil e de fácil digestão, ela se tornou também a linguagem favorita para introduzir novas pessoas ao mundo da programação, fazendo milhares se apaixonarem e com ela ficam.
Não à toa ela é a terceira linguagem mais usada no mundo, segundo [pesquisa do StackOverflow](https://stackoverflow.blog/2023/06/13/developer-survey-results-are-in/) 

E hoje vamos aprender um pouco mais dessa linguagem amada e infame entre os programadores, e descobrir como e porque ela se tornou tão usada. 

## Python não é uma linguagem de programação!

*Como assim, você acabou de dizer que era. Quer dizer que eu to programando em quê? Inglês?*

Bem, de certa forma sim!

Python nada mais é do que um conjunto de propostas e convenções, as chamadas PEPs (Propostas de Aprimoramento do Python, em português) que dentro de si definem qual a implementação da linguagem de programação Python. Isso quer dizer que se você quiser, pode fazer uma implementação independente, porém para ser dita uma implementação devida de Python, ela deve cumprir com as quase 800 PEPs. 

*Então o que é aquele .exe que eu baixo quando eu vou no site do python?* 

Aquele é uma das várias implementações do interpretador Python. Podemos dizer que é a "oficial" chamada de CPython, que como o nome pode entregar, é implementada usando a linguagem C.

Mas não é a única implementação, sendo as mais famosas:

- Jython: Uma implementação que usa a máquina virtual do Java como base
- RustPython: Implementação de Python criado com a linguagem Rust, que pode ser usado [no navegador](https://rustpython.github.io/demo/) e com projetos Rust
- PyPy: Um interpretador Python com compilação *Just In Time* (JIT)
- IronPython: Interpretador Python usando a *Common Language Runtime* do C#
- PyJs: Python implementado usando JavaScript (pra variar)

Apesar de cada um trazer suas vantagens e desvantagens, dificilmente você precisará usar qualquer outra versão senão a oficial da Fundação Python. Mas se um dia a curiosidade bater, baixe algumas dessas outras implementações e brinque um pouco com elas!

## Para o que se usa Python?



## A Parte Feia do Python

Uau, depois dessa introdução Python parece ser melhor coisa que já pisou nessa terra, não é? É, mais ou menos. 

Apesar dos seus positivos quase massacrar seus pontos negativos, eles ainda existem e devem ser considerados. Não caia na tentação de seguir a Lei de Atwood: 

> "Tudo que pode ser escrito em JavaScript, um dia será."

Apesar de se referir a JavaScript, ela se encaixa supreendentemente bem no ecossistema de Python, que é tão usado (se não mais) que JavaScript. E apesar de ser uma regra semi-sarcástica, ela é seguida com esmero pelas pessoas, que tem um hiperfoco em uma única linguagem de programação e querem fazer absolutamente tudo com aquela mesma linguagem. 

Python tem alguns problemas fatais que vem com a sua simplicidade e facilidade como mantra, e que devem ser consideradas durante a escolha como a tecnologia para um projeto sério. Sendo alguns deles:

- **Performance:** Python é extremamente lento em comparação a linguagens compiladas como C, C++ ou até mesmo Java. Apesar de muitas bibliotecas usarem uma API escrita em C por debaixo dos panos, código puramente em Python é lento em algumas ordens de magnitude (até 100x mais devagar em alguns casos) por ser uma linguagem interpretada e de tipagem dinâmica. 
- **Uso de Memória:** Por ser interpretada, ela também usa muito mais memória para rodar o interpretador em conjunto com a memória do próprio programa (diz-se que ela tem um *overhead* de memória maior), que pode ser um empecilho para sistemas sensíveis a memória.
- **O "Inferno de Dependências":** Em projetos maiores, as dependências de um programa Python se torna uma grande dor de cabeça, uma vez que o gerenciador de pacotes PIP não se dá bem em desemaranhar esses problemas.
- **Dificuldade com Paralelismo:** O Python possui um problema chamado de *Global Interpreter Lock* (GIL) que impede o intepretador de ter múltiplas threads executando código Python simultaneamente no mesmo processo. O que faz paralelismo na linguagem seja bastante limitado, em comparação com linguagemns que a possem nativamente como Go ou Rust.

A lista até pode ser pequena de desvantagens, mas não deixe se enganar, em larga escala ela se tornará uma dor de cabeça sem tamanho. Lembre-se:

**Em programação não existe uma solução milagrosa para seus problemas, estude os casos de uso de uma linguagem antes de usá-la em um projeto.**

Tudo isso para dizer: pelo amor de deus parem de usar Python pra fazer jogos e aplicativos mobile, aprendam uma outra linguagem de programação, eu imploro. 

## Preparação de um Ambiente Python

**TODO**


## Referências (em ordem de aparição)

https://stackoverflow.blog/2023/06/13/developer-survey-results-are-in/

https://peps.python.org/

https://wiki.python.org/moin/PythonImplementations

