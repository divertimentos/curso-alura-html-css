# Curso: HTML5 e CSS3

# Parte 1: A primeira página web

![screenshot](https://github.com/guiemi-learning-center/Curso-HTML-CSS-Alura/blob/master/screenshot.jpg)

## Hexadecimais

* Hexadecimais utilizam o dicionário: **0123456789** e **ABCDEF**;
* o padrão RGB (Red, Green e Blue)
* Uma hashtag seguida de 6 slots:

  * `#_ _ _ _ _ _`
* O **0 (zero)** é a ausência de cor e o **F (full)** é o máximo de cor

### Montando as cores

#### Hexadecimal

Se você quer, então, fazer o preto, faça **dois zeros** para o vermelho, **dois zeros** para o verde e **dois zeros** para o azul:

* `#000000`

Branco:

* `# FFFFFF`

Vermelho:

* `#FF0000`

Cinza (AB**C**DEF):

* `#CCCCCC`

#### RGB

O dicionário RGB tem 256 cores, começando do 0 (zero). Sua sintaxe é:

* `rgb(red, green, blue);`

Então, para fazer o branco:

* `rgb(255, 255, 255);`
* `rgb(0, 0, 255);`

***

# Parte 2: Posicionamento, Listas e Navegação

* Para colocar uma imagem como background, basta usar a sintaxe:

  ```css
  footer {
    background: url("assets/produtos/bg.jpg");
  }
  ```

* Para colocar o "c" comercial usando Unicode, basta:

# Parte 3: Trabalhando com formulários e tabelas

* Lembrar que o `id` do <input/> faz par com o `for`do <label/>. Eles sempre andam juntos.
* O <input> cujo type é "submit" mostra um botão de enviar com "submit query" como nome default. Para mudar o texto dentro do botão, basta usar um `value="Nome do "`
* Quando você passa um `name` para um grupo de inputs do tipo radio, eles passam a dar "check" em apenas um de cada vez, como irmãos.

#### Hierarquia de prioridade dos seletores
A hierarquia de preferências é `id` --> `class` --> `tag`. Pode-ser inferir que um `form p` tem preferência sobre um simples `p`, mas não sobre uma classe.

O único mais forte que o `id` é o estilo inline (`style` no próprio HTML).

# Parte 4: Avançando no CSS
* Aprendi sobre como usamos o float para flutuar uma imagem deixando uma "sombra/traço" no local original para evitar que o conteúdo em volta a sobreescreva.
* Para modificar a primeira letra, temos o pseudoelemento `::first-letter {}`. Para a primeira linha em um parágrafo, temos a `::first-line {}` 
* Também aprendi a usar o `::before {}` e o `::after {}`

### Seletores Avançados
* Usamos o `>`para selecionar apenas filhos diretos de um elemento
* Da mesma forma, usamos o `+` para selecionar um irmão de um elemento
* Para selecionar todos os irmãos, usamos o `~`

Os seletores avançados têm a mesma força na hora de sobreescrever.

Para selecionar tudo exceto uma classe, usamos o `:not(#className)`

### calc()

