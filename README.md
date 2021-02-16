# HTML e CSS

# Sobre o repositório e como colaborar

Criei esse e (irei criar outros) repositórios no GitHub com a intenção de compartilhar meus aprendizados, servindo quase que como uma mini documentação da tecnologia em questão.

Sinta-se livre para abrir **issues** caso encontre qualquer tipo de erro, seja de escrita, alguma informação incorreta/incompleta, etc, informando aonde está o erro e a correção ou uma sugestão de correção.

Estarei escrevendo quase que diariamente melhorias e adições ao repositório, lembrando que minha intenção é criar um repositório que se aprofundará com o tempo, não viso recriar completamente a documentação do HTML (ou outra tecnologia) em português.

Como maior fonte de informação, utilizei os tutoriais e documentação da [W3Schools](https://www.w3schools.com/), a qual citarei de vez em quando. Acredito que **juntos** podemos criar um ótimo repositório para que desenvolvedores possam se aperfeiçoar, conferir ou aprender coisas novas!

# HTML

**HTML** significa **Hyper Text Markup Language** (Linguagem de Marcação de Hipertexto), tendo sido inicialmente **lançado em 1993**, sendo sua versão mais recente o HTML5 (versão 5), sendo a linguagem padrão para a criação de websites como a estrutura do seu conteúdo.

O **HTML** funciona a partir de “blocos”, que podem ser auto-contidos, esses que eu chamarei de tags, ou que precisam de uma tag de abertura e fechamento com algum conteúdo inserido, que chamarei de elementos.

 

## Estrutura base

Todo documento HTML terá uma estrutura base como essa abaixo, que é uma das partes fundamentais para se criar um website funcional:

```html
<!DOCTYPE html>
<html lang="pt">
	<head>    
		<meta charset="UTF-8">    
		<meta name="viewport" content="width=device-width, initial-scale=1.0">    
		<title>Alê Pizzas</title>
	</head>
	<body> 
	</body>
</html>
```

**`<!DOCTYPE html>`** especifica que é um documento **HTML**.

**`<html></html>`** engloba toda a sua marcação.

**`<head></head>`** informações sobre o seu site, que são acessadas por mecanismos de busca e o navegador e não são visíveis ao usuário final. Geralmente a conexão com arquivos **CSS** e **JS** são feitos aqui.

**`<meta>`** inclui informações principalmente acessadas pelos mecanismos de busca, tornando o seu site mais visível.

**`<title></title>`** adicionado dentro da sua **head**, o texto que estiver inserido como conteúdo se tornará o título de sua página, que aparece na parte superior do navegador.

**`<link rel="" href="">`** faz a conexão entre dois documentos, o atributo **rel** significa relationship, basicamente pergunta o que é o arquivo que estamos conectando, por exemplo, quando for um arquivo **CSS**, utilizamos **stylesheet**, ou quando for um ícone que aparecerá em cima da página, **icon**. Já o **href**, é onde especificamos o caminho (local) do que queremos conectar.

**`<body></body>`** elemento que englobará todo o conteúdo visível ao usuário da sua página.

### **Atributos importantes da tag meta:**

A tag **meta** é **importantíssima**, pois é nela onde são feitas alguns ajustes para tornar o website mais acessível a usuários de dispositivos móveis e é feita a otimização para mecanismos de busca, famosamente conhecido como **SEO**, vulgo **Search Engine Optimization (Otimização para Mecanismos de Busca)**.

Dentro da tag, podemos adicionar dois atributos: **name** e **content**. O atributo name serve para definir um nome para o **metadado**, que será lido pelo navegador ou mecanismo de busca e servir para uma função específica, já o **content** será o conteúdo associado ao **metadado** definido em **name**, ****como podemos ver nesses exemplos:

Adiciona uma descrição ao seu website, vista nos mecanismos de busca.

```html
<meta name="description" content="A maior pizzaria à moda alemã do mundo!">
```

Especifica um charset (conjunto de caracteres) a ser utilizado, o utf-8 é recomendado.

```html
<meta charset="utf-8">
```

Define o comportamento do enquadramento da sua página, tornando-o mais acessível para certos dispositivos.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

Determina como os mecanismos de busca irão tratar seu site, nesse caso, indexar a página e seus links. 

```html
<meta name="robots" content="index, follow">
```

Atribui palavras-chave para o seu site ser melhor encontrado e recomendado em mecanismos de busca.

```html
<meta name="keywords" content="pizza barata, alemã, alê pizzaria">
```

## Formatação

No HTML há vários elementos que permitem você "formatar" o texto, **o seu uso principal é para gerar hierarquia de importância de cada elemento**, e **não ditar o estilo do website**, que no caso é feito com **CSS**.

### Títulos

Os títulos são adicionados através dos elementos **h**, de 1 à 6. Como a pouco avisado, tem o objetivo de gerar hierarquia, e não de propriamente estilizar o website. De 1 à 6 o tamanho vai diminuindo, como abaixo exemplificado:

# Título H1

```html
<h1>Título H1</h1>
```

## Título H2

```html
<h2>Título H2</h2>
```

### Título H3

```html
<h3>Título H3</h3>
```

### Título H4

```html
<h4>Título H4</h4>
```

### Título H5

```html
<h5>Título H5</h5>
```

### Título H6

```html
<h6>Título H6</h6>
```

### Parágrafos e Outros Elementos

No HTML você pode inserir parágrafos através do elemento **p**, servindo como divisão para os textos. Além disso, você pode atribuir algumas formatações extras com os outros elementos explicados abaixo juntamente:

```html
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
```

**`<b></b>`** transforma o texto inserido em negrito, utilizado para chamar atenção.

**`<strong></strong>`** além de transformar em negrito, é utilizado para marcar coisas de grande importância.

**`<i></i>`** deixa o texto inserido em itálico, geralmente utilizado para expressar temos técnicos, outras linguagens e pensamentos.

**`<em></em>`** além de deixar em itálico, é utilizado para criar ênfase.

**`<mark></mark>`** deixa o texto marcado, destacado.

**`<small></small>`** deixa o texto pequeno, se utiliza principalmente para avisos de direitos autorais e comentários adicionais.

**`<del></del>`** torna o texto riscado, indicando que foi removido do texto.

**`<ins></ins>`** sublinha o texto, indicando que foi inserido ao texto.

**`<sub></sub>`** o texto se torna subscrito, geralmente utilizado para escrever fórmulas químicas.

**`<sup></sup>`** o texto se torna sobrescrito, geralmente utilizado para se escrever fórmulas matemáticas e notas de rodapé.

**Exemplo:**

```html
<p><strong>Bem-vindo à Alê Pizzas!</strong>Temos uma grande variedade de <i>pizzas alemãs</b> com um preço mais do que <mark>saboroso!</mark></p>
```

## Imagens e Vídeos

### Imagens

Imagens são uma parte fundamental de vários websites e podem ser facilmente inseridos no seu documento HTML, como demonstrado abaixo com a tag **img**:

```html
<figure>
	<img src="/pizza.jpg" alt="Pizza de mussarela">
	<figcaption>Pizza de mussarela por R$13,99</figcaption>
</figure>
```

Como pode ser visto, a tag **img** é englobada de um elemento **figure** que apesar de não ser obrigatório se é recomendado, pois deixa o site melhor estruturado e permite o uso do **figcaption**, outro elemento que adiciona uma descrição para a imagem.

O atributo **src** é onde você colocará o caminho de sua imagem, e o **alt** é tão importante quanto, pois diz o que é aquela imagem, permitindo usuários de leitores de tela entenderem as imagens, tornando o site mais acessível. **O uso do atributo alt é considerado uma boa prática, sua diferença para o figcaption é que ele é utilizado para descrever detalhes da imagem ou algo relacionado a mesma.** Também pode ser inserido uma altura e largura fixa à imagem através dos atributos **width** (largura) e **height** (altura) utilizando-se pixels como medida, apesar de que muito pode calhar configurar isso através do CSS.

### Vídeos

Vídeos, assim como imagens, podem ser inclusos em um website com uma enorme facilidade através do elemento **video**, além de algumas funcionalidades extras para melhorarem a experiência. A sintaxe sendo:

```html
<video controls width="1280" height="720" src="/video.mp4"></video>
```

Como visto, vídeos também podem receber os atributos **width** e **height**. Além disso, para fazer o seu vídeo controlável, utilize o atributo **controls**, que adiciona um botão de iniciar/pausar, uma barra para passar entre momentos do vídeo e um controle de volume. O atributo **autoplay** também pode ser adicionado, fazendo o seu vídeo tocar automaticamente quando o vídeo carregar.

Caso você deseje, você pode incluir mais de uma fonte (source) para o seu vídeo, caso o navegador do usuário, ou o vídeo em questão não esteja funcionando propriamente por algum motivo. Para isso, utilize-se da tag **source** dentro do elemento **video**:

```html
<video width="1280" height="720" autoplay>
	<source src="video.mp4" type="video/mp4">
  <source src="video.ogg" type="video/ogg">
	Erro ao disponibilizar vídeo, considere reiniciar a página ou atualizar seu navegador.
</video>
```

Foi adicionado um pequeno texto de erro no final da tag **video**, que é mostrado apenas quando nenhuma das fontes do vídeo funciona. Também há a adição do atributo **type**, para especificar o formato do vídeo, sempre seguindo o padrão **video/[extensão do arquivo de vídeo]**. As fontes dos vídeos serão utilizadas de acordo com a ordem, ou seja, apenas há chance da segunda fonte ser mostrada caso a primeira não funcione, assim por diante.

## Links e Âncoras

Algo de muita importância também são os links, que conectam diferentes páginas, ou diferentes partes de uma página de forma bem intuitiva através do elemento **a**:

```html
<a href="https://www.w3schools.com/tags/tag_a.asp" target="_blank">Veja mais sobre a tag a</a>
```

Através do atributo **href** você colocará o link de destino, e com o atributo **target** você irá indicar um comportamento, no caso, quando o atributo estiver ausente, ele abrirá na mesma aba, mas como temos **_blank** como valor, ele irá abrir em uma nova aba.

Vale lembrar que o elemento **a** pode ser combinada com outras coisas, por exemplo, pode-se utilizar emojis e até outros elementos **HTML**. Olhe só, clique nesse emoji: [😀](https://emojipedia.org/)

Apesar do elemento **a** ser muito útil como uma forma de disponibilizar links mais fácil e agradavelmente, isso não reflete todo seu potencial, que pode ser alcançado utilizando o elemento **a** para o propósito de seu nome: uma âncora. Uma âncora conecta duas partes da mesma página, como no exemplo abaixo:

```html
<p id="#empresa">Sobre a empresa</p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
<p>Funcinários</p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
<a href="#empresa">Volte as informações da empresa</a>
```

O **id** é um atributo que serve para identificar exclusivamente um elemento/tag do documento e assim o acessar posteriormente, por exemplo, através de **JavaScript** ou como no exemplo dado, para criar uma âncora, ou seja, é um **href** válido, então quando clicado, a sua página automaticamente irá para a localização em questão, tornando a navegação mais intuitiva.

## Formulários

Outra das funcionalidades básicas e fundamentais do **HTML** são os formulários, que te permitem lidar com a inserção de informações por parte do usuário e o envio das mesmas, sendo essa segunda parte deixada de lado por aqui, já que dependeria de uma linguagem como **PHP** ou **JavaScript** para ser melhor explicada, mas a título de curiosidade, pesquise sobre o atributo **action** adicionado no elemento **form**. A seguir, utilizarei esse código como um exemplo:

```html
<form>    
	<h4>Registre-se</h4>    
	<label for="username">Nome de usuário</label>
<br>    
	<input name="username" type="text" id="username" placeholder="Insira seu nome"/>
<br>    
	<label for="useremail">E-mail</label>
<br>    
	<input name="useremail" type="email" id="useremail" placeholder="Insira seu e-mail"/>    
<br>    
	<label for="userpassword">Senha</label>
<br>    
	<input name="userpassword" type="password" id="userpassword" placeholder="Insira uma senha forte"/>    
<br>    
	<button type="submit">Finalizar cadastro</button>
</form>
```

Como visto, vários novos elementos e tags foram apresentados, além de atributos, o que fará essa sessão um pouquinho longa (irei explicando por partes).

O elemento **form** serve como um enquadramento de todas as entradas de informação de um formulário específico, ou seja, para a sua tela de login utilizaria-se um **form**, e para a de registro, outra, e por assim vai. Bom, pode-se fazer uma analogia bem simples de que cada **form** que você inserir será uma pesquisa diferente. No **form** também pode-se adicionar o atributo **autocomplete**, onde você pode definir se o seu formulário vai auto-completar informações armazenadas no navegador do usuário ou não, através dos valores **on** e **off**, respectivamente. O atributo **autocomplete** também pode ser adicionado nos **inputs** - que irei explicar logo embaixo - individualmente, controlando mais precisamente seu comportamento.

Também foi apresentado a tag **br**, que simplesmente gera uma quebra de linha, para que o formulário não ficasse muito visualmente confuso sem o uso de **CSS**.

### **Label**

O elemento **label**, geralmente traduzido como rótulo ou legenda, exerce uma simples funcionalidade de especificar que tipo de **input** é preciso, ou seja a informação que é necessária. O atributo **for** serve para conectar o **id** de uma entrada com o seu devido rótulo, conexão esta que pode ser facilmente visualizada no momento em que você clica no rótulo, por exemplo, “E-mail”, o **input** que estava conectado com ele através do **for** e do **id** é selecionado.

### **Input**

O **input** é sem dúvidas a tag mais utilizada entre os tipos de formulário, sendo acompanhado de um atributo **name**, que garante que essa informação seja enviada posteriormente de forma identificável (ou seja, será mais fácil tratar essa informação depois no seu **back-end**). Também geralmente se acompanha de um atributo **id** para colocar-se sua identificação e se conectar com sua **label**.

O atributo **type** é muito importante, pois permite vários tipos de verificações sem a necessidade de utilizar outras linguagens para isso. Como por exemplo, caso o valor do atributo seja **email**, é necessário um @ na informação digitada pelo usuário para ser válido, se não, quando o usuário clicar para submeter o formulário, vai indicar o problema e o mesmo não será realmente enviado, ou no caso do valor ser **password**, o texto será escondido, para evitar que outras pessoas simplesmente vejam a senha enquanto você a escreve, apesar de não proteger a senha de ser descoberta. Fortemente recomendo a leitura da página sobre os diferentes tipos de **type** para o elemento **input** na [W3Schools](https://www.w3schools.com/html/html_form_input_types.asp).

É muito bom saber também sobre o atributo **required**, pois nele é possível definir se um campo é obrigatório ou não. Ou seja, caso o campo seja obrigatório e não seja preenchido, o mesmo não será enviado, e demonstrará uma mensagem de erro.

Caso você tenha requisitos extras sobre o tamanho de um certo campo, como uma senha, você pode aproveitar-se dos atributos **minLength** e **maxLength** que recebem como valor um número que especifica a quantidade de caracteres de mínimo e máximo, respectivamente.

### **Button**

O elemento **button** é simples, gera um botão clicável que executa uma função quando o mesmo é executado, tal função pode ser definida através de um valor para o atributo **type**, como por exemplo o valor **submit**, que envia as informações do formulário em que o mesmo está inserido.

Também é possível executar **JavaScript** usando eventos como **atributos** e um pedaço de código **JavaScript** como valor desse atributo. Veja mais sobre esses eventos na [W3Schools](https://www.w3schools.com/tags/ref_eventattributes.asp).

### **Dropdown: Select e Option**

Utilizando-se dos elementos **select** e **option** é possível fazer uma **dropdown**, que seria como selecionar uma opção de uma lista, muito utilizado no ramo dos formulários, tendo uma sintaxe bem simples.

```html
<select name="culinariafavorita" id="culinariafavorita">    
	<option value="francesa">Culinária Francesa</option>    
	<option value="chinesa">Culinária Chinesa</option>    
	<option value="indiana">Culinária Indiana</option>    
	<option value="italiana">Culinária Italiana</option>    
	<option value="turca">Culinária Turca</option>
</select>
```

O atributo **select** especifica que estamos falando de um **dropdown**, aceitando dentro de si quantos elementos **option** quiser, que vem acompanhado de um atributo **value**, que diz qual será o valor dessa escolha no back-end quando o formulário for enviado, pois o texto entre as tags serve apenas na questão visual.

### **Textarea**

Um elemento bem simples de se explicar e que também é bem útil é o **textarea**, que cria algo semelhante a um input, porém, com a intenção de comportar textos maiores, como por exemplo uma crítica ou como parte de uma pesquisa, como demonstrado abaixo:

```html
<textarea name="critica" id="critica" cols="30" rows="10"></textarea>
```

Sem muitos segredos, é assim que o **textarea** funciona. Como pode ter notado, os atributos **cols** e **rows** são novos, e com eles você pode definir o tamanho em colunas e linhas, respectivamente, fazendo seu **textarea** ter o tamanho que melhor se adequa à situação.

## Listas

Com o HTML há também a possibilidade de se criar múltiplas **listas**, **ordenadas** ou **sem ordem**, que pode ser feita facilmente, utilizando a tag **ul** e **ol** respectivamente. Essas tags englobam uma certa quantidade de tags **li**, que são os itens da lista, como nesse exemplo:

```html
<ol>
  <li>Maça</li>
	<li>Banana</li>
	<li>Laranja</li>
</ol>
```

Esse exemplo utilizou uma **ol**, no caso de uma **ul** os itens da lista seriam adicionados com uma pequena bolinha preta ao lado, que pode ser modificada utilizando **CSS**. Inclusive, você pode utilizar outras **ol** ou **ul** dentro de uma, ou adicionar outros elementos na tag **li**, muito comumente combinando-se os elementos **li** e **a** e uma pitada de **CSS** para se criar algo como um cabeçalho de navegação.

## Tabelas

Tabelas, como aquelas que você encontra no Excel podem ser criadas também no HTML, com o uso dos elementos: **table** - que engloba todos os outros itens de uma tabela -, **tr**, que cria uma linha de células, **th** - que indica o cabeçalho de uma coluna da tabela - e **td**, que seria uma célula de dados comum.

```html
<table>
    <tr>
    	<th>Nome</th>
			<th>Sobrenome</th>
			<th>Idade</th>
      <th>Ocupação</th>
    </tr>
    <tr>
    	<td>Mark</td>
      <td>Daniel</td>
			<td>16</td>
			<td>Estudante</td>
    </tr>
</table>
```

O que foi escrito em **th** sempre ficará centralizado e em negrito, já o que for escrito em **td** estará sempre orientado a esquerda por padrão.

## Elementos Semânticos

Adicionados na versão 5 do HTML, os **elementos semânticos** servem como uma forma de **organizar** o seu website em **propósitos,** tornando mais fácil navegar entre o código para **futuras correções** de determinadas áreas, como o cabeçalho ou a parte principal do website. Anteriormente, quando o HTML não possuía os **elementos semânticos**, se usava principalmente o elemento **div** para englobar diversas partes do site, porém era muito mais difícil navegar posteriormente no código e também complicava a vida na hora de fazer o CSS.

Em sessões anteriores já exploramos alguns elementos semânticos, como o **table**, **figure** e **form**, e abaixo, esses são outros **principais elementos semânticos**:

**`<header></header>`** utilizado para o cabeçalho de websites, onde geralmente se tem a logo do site ou como cabeçalho de notícias ou blogs.

**`<footer></footer>`** serve como o rodapé do seu site, muitas vezes é onde há um dicionário de links do website ou alguma mensagem de direitos autorais ou de quem criou.

**`<nav></nav>`** é aonde se encontra qualquer tipo de navegação, como uma lista de links, por exemplo.

**`<main></main>`** especifica qual seria o conteúdo principal do seu website, o que deve ser o centro das atenções, como por exemplo, em um site de um restaurante, pode ser o menu.

**`<section></section>`** determina uma seção, por exemplo, em um website de notícias, cada section pode representar uma categoria de notícias, como esportes, economia e curiosidades.

**`<article></article>`** como o section funciona como a categoria de notícias no exemplo, o article seria cada uma dessas notícias específicas, ou uma postagem de um blog em outro contexto.

**`<aside></aside>`** funciona como um conteúdo relacionado, algo que está ao lado do conteúdo principal, como por exemplo, em um site de notícias, pode ser informações do autor da reportagem, ou em um blog, uma lista de postagens parecidas, por exemplo.

## Entidades HTML

No HTML, alguns caracteres podem **causar problemas com o código**, pois são interpretados de forma diferente, como o caso do sinal < e >, por exemplo, que representa a criação de uma nova tag/elemento no código. Além disso, podemos nos esbarrar querendo adicionar caracteres especiais, como um **símbolo de** **copyright**. Para evitar isso, há entidades HTML.

As entidades podem ser adicionadas através de **nomes**, utilizando-se **&(nome_da_entidade)** ou códigos, com **&#(número_da_entidade)**. Apesar de nomes serem mais fáceis de se decorar, há menos compatibilidade com navegadores, o que pode ser um problema, se o seu website precisar ser compatível com computadores que tenham navegadores defasados.

Um grande exemplo de **entidade HTML** é o **&nbsp** (non-breaking space), que te permite criar quantos espaços quiser em um texto, já que muitos navegadores acabam removendo os espaços quando há mais de um. Há **centenas de entidades HTML**, que torna impossível de colocá-los todos aqui, porém **listas completas** **podem ser encontradas na internet**, e claro, **você não tem a obrigação de decorá-los**, deixe que com o tempo e experiência você decore alguns dos que forem mais importantes.

# CSS

**CSS** significa **Cascading Style Sheets** (Folhas de Estilo em Cascata), sendo a **linguagem padrão** para a **estilização** de websites, controlando como o HTML é demonstrado na página. Foi lançado em **17 de dezembro de 1996** e sua versão mais recente é o CSS3.

O **CSS** funciona a partir de **seleção**, **propriedade** e **valor**. Selecionamos um tipo de elemento, ou um caminho de um elemento, ou até mesmo um elemento específico e a partir disso começamos a mudar a aparência de um website.

## Formas de se adicionar código CSS

Há **3 formas de se colocar código CSS** em um documento HTML, seja **em linha**, seja **internamente** ou **externamente**. É possível ter código CSS das 3 maneiras em seu código, podendo um sobrescrever mudanças do outro. O com maior prioridade é o **em linha**, que é diretamente inserido no elemento, depois **internamente**, que já está no mesmo arquivo que o HTML e por fim, **externamente**, que está em outro arquivo, veja abaixo como cada um deles funciona:

### **Em linha**

A partir de um elemento HTML que você já tenha, você pode adicionar o atributo **style**, e a partir dele colocar o código **CSS**. Esse método é pouco recomendado, pois além de tornar o documento HTML mais "**bagunçado**", você precisa utilizar o atributo para cada elemento **individualmente**, o que torna muito mais trabalhoso e mais **difícil de se fazer mudanças** posteriormente. Exemplo:

```html
<h1 style="color: white; font-weight: bold;">Sobre a empresa</h1>
```

### **Internamente**

Para se adicionar **CSS** internamente, será utilizado o elemento **style** - **não confundir com o atributo style!** -, onde você poderá escrever CSS da mesma forma com que você escreve externamente, porém com a **desvantagem** de que o seu arquivo HTML irá ficar **muito maior**, e chegará a um ponto que se tornará **ineficiente** mudar o CSS dentro do HTML. O elemento **style** geralmente é colocado na **head**, para ser carregado inicialmente com o site, já que é com o intuito de modificar algo do CSS externo, porém você também pode **optar por colocá-lo no final**, dependendo da situação. Para exemplificação:

```html
	<head>
		<style>
			h1 { 
				color: red;
			}
		</style>    
		<meta charset="UTF-8">    
		<meta name="viewport" content="width=device-width, initial-scale=1.0">    
		<title>Alê Pizzas</title>
	</head>
```

### Externamente

Sendo a **forma mais recomendada** de se utilizar o **CSS**, é preciso adicionar uma tag **link** no seu código HTML, conectando seu **arquivo .css** ao HTML, assim:

```html
<link rel="stylesheet" href="/style.css">
```

 

Além da tag **link**, você precisa claro, criar um **arquivo .css**, onde o código CSS irá ficar, geralmente você pode colocar na mesma pasta onde está o HTML sem nenhum problema. E da mesma forma como o elemento **style**, você pode optar por colocar esse **link** no início ou no fim do documento, mudando a **prioridade de carregamento**.

Com o uso de **CSS externo**, você pode dividir o seu código CSS em **diversos arquivos**, e colocar diferentes prioridades de carregamento para tornar o site mais rápido, apesar de **não ser uma técnica recomendada** para **iniciantes**. Ou seja, **não se preocupe** de ter todo o seu código CSS em 1 arquivo por agora.

## Sintaxe

A **sintaxe do CSS** é simples, como anteriormente "spoilado" em outras seções, ela se pode ser resumida em **seleção**, **propriedade** e **valor**, veja nesse exemplo:

```css
seleção {
	propriedade-1: valor-1;
	propriedade-2: valor-2;
}
```

Podemos ver onde se localiza cada "peça do quebra-cabeça", a **seleção** pode ser **um** elemento ou **vários**, de acordo com o **seletor** usado, que iremos nos aprofundar mais a frente. A **propriedade** é uma **característica** que queremos mudar do(s) elemento(s) selecionados, alguns exemplos são: margin, padding, width, height, font-weight, color, e por aí vai, muitas propriedades possuem formas específicas de **valor**, por exemplo, em color, o valor pode ser tanto o **nome de uma cor**, **um valor RGB** ou até um **código** **HEX**, já **width**, entende unidades de medidas suportadas no CSS. **Iremos explorar progressivamente diferentes propriedades do CSS** e como elas funcionam, mas como há uma **infinidade de propriedades**, e essas com **funcionamentos diferentes**, sirva-se de uma boa pesquisa no Google.

## Seletores

No CSS há **vários seletores,** que te permitem fazer **seleções precisas** do que você deseja modificar, esses seletores ficam em "**seleção**" no exemplo de sintaxe feito acima, esses são os principais seletores:

**`*`** seleciona todos os elementos do documento HTML.

**`(elemento)`** seleciona todos os elementos com o nome inserido, por exemplo "h1".

**`(elemento), (elemento)`** seleciona todos os elementos X e todos os elementos Y.

**`(elemento) (elemento)`** seleciona todos os elementos Y dentro de todos os elementos X.

**`(elemento) > (elemento)`** seleciona todos os elementos Y que são parentes de um elemento X.

**`elemento + elemento`** seleciona o primeiro elemento Y dentro de elementos X.

**`.(classe)`** seleciona todos os elementos com o nome da classe inserido, por exemplo ".nome".

**`(elemento).(classe)`** seleciona todos os elementos do nome inserido que possuem a classe inserida.

**`.(classe).(classe)`** seleciona todos os elementos com ambas as classes inseridas.

**`#(id)`** seleciona o elemento com o ID inserido, por exemplo "#logo".

## Especificidade

Uma das **características** **do CSS**, que faz parte seu nome, é a **cascata**, isso significa que, caso você modifique o mesmo **elemento e propriedade** mais de uma vez no CSS, em suma, a modificação que estiver mais em baixo será a utilizada, sobrescrevendo a que estiver em cima, pois o CSS "**lê**" de **cima para baixo** o código. Além disso, vale lembrar de como a forma **em linha** é mais priorizada do que **internamente**, que é mais priorizada do que **externamente**.

Além disso, há algumas outras peculiaridades, uma forma fácil de se pensar nisso é de acordo com o "**quão único**" é uma seleção, por exemplo, caso selecionemos apenas todos os elementos **h1** de um documento, obviamente, será menos único do que a seleção de uma classe "**cabeçalho**", que será menos única do que a seleção de um **id**, que possui alta prioridade por exatamente existir **apenas 1 elemento** com certo **id** pelo documento. Pensando nisso, mesmo que uma modificação usando **classe** como seleção esteja acima de uma modificação que **apenas seleciona** o elemento, a que utiliza classe ainda será priorizada. A maioria das **IDE's** possuem um visualizador de prioridade, bastando apenas passar o mouse por cima da seleção, mas para melhor demonstração, veja os exemplos:

**`(elemento)`** prioridade (0, 0, 1)

**`.(classe)`** prioridade (0, 1, 0)

**`(elemento).(classe)`** prioridade (0, 1, 1)

`**#(id)`** prioridade (1, 0, 0)

Caso ainda tenham sobrado dúvidas, a junção de diferentes formas de seleção, como (elemento).(classe), irá "**somar**" a prioridade de ambos, que é dividida em 3 partes, no caso, o (x, x, x), uma forma de **visualizar melhor** o "**quão importante**" é a seleção é comparando os números, por exemplo, uma seleção (1, 0, 0), ou seja, com "100" de prioridade, é maior do que a seleção (0, 1, 2), que seria "12". 

Em **casos muito extremos**, você pode se deparar com a impossibilidade de modificar um elemento, muitas vezes ocasionada por uma **falta de uma metodologia** ou **organização** do código CSS em que você está trabalhando, para mudar isso, apesar de ser **nem um pouco recomendado**, você pode adicionar **!important** ao lado de uma propriedade, para assim, sobrescrever, o que seria a maior prioridade de todas, veja:

```css
header {
	background-color: red !important;
}
```

## Box Model

**Todos os elementos** de uma página web são representados graficamente como se estivessem numa **caixa** (box), isso pode ser visto principalmente nas **ferramentas de desenvolvimento** e **inspeção** dos **navegadores da web**. Conhecer o **Box Model** ou **Modelo de Caixa** em português, é **fundamental** para entender melhor como os elementos se comportam, e evitar cair em problemas com o tamanho de certos elementos. Veja essa imagem demonstrativa:

![Box Model](https://i.imgur.com/g9PwA80.png)

Como podemos ver na imagem, o **verdadeiro** "**tamanho**" de um elemento não é apenas sua **altura** e **largura**, além disso, é a soma de seu **padding** (preenchimento) e **border** (borda). A **maioria dos elementos** já vem com algumas propriedades de **margem**, **borda** e **preenchimento** definidas, mas isso pode ser modificado, alias, **é uma prática bem comum** no início de um código CSS **selecionar todos os elementos** com o seletor "*****", e definir as propriedades **margin** e **padding** como 0, já que navegadores por padrão definem uma certa **margem** indesejável.

Uma dica interessante é utilizar-se da propriedade **box-sizing** em seus sites, com o valor "**border-box**". Assim, ao invés de você sempre precisar calcular o tamanho e modificar a altura e largura de um elemento, o **padding** e **border** não irão aumentar o tamanho final, eles serão "aparados", e com o tamanho que você já definiu de **width** e **height** corretamente, como se o navegador automaticamente calculasse isso para você. **É completamente aceitável aplicar isso para todos os elementos, não há nenhuma desvantagem**.

Como antes explicado, o **padding** é como se fosse o **preenchimento** de um elemento, geralmente serve por exemplo, para criar espaços internos para que conteúdo como texto não fique "grudado" no canto da página, o que de certa forma dificulta a leitura.

Já a **margin**, ao invés de criar um preenchimento interno como o **padding**, cria um espaçamento externo, dividindo um elemento de outros.

Para ambos **margin** e **padding**, é possível modificar o seu tamanho facilmente com algumas propriedades, no caso, utilizarei um de **padding** e um de **margin** como exemplo no código, mas as mesmas propriedades existem tanto para um quanto para o outro, modificando-se apenas o nome:

```css
div {
	padding: 30px 50px;
	margin-top: 10px;
	margin-left: 15px;
	margin-right: 20px;
	margin-bottom: 25px;
}

```

Podemos ver nesse exemplo, como podemos modificar individualmente cada lado com valores diferentes através do **top**, **left**, **right** e **bottom**, que é muito bom quando precisamos modificar apenas um lado.

Além disso, podemos modificar vários lados através de uma só propriedade, a **margin** e/ou **padding** sem especificar um lado, que aceita 1, 2, 3 ou 4 valores. Quando apenas um valor é dado, ele será válido para os 4 lados do elemento, ou seja, **todos os lados terão** 10px de **padding**, por exemplo. Com 2 valores, o primeiro será de cima e em baixo, e o segundo para a esquerda e direita. Com 3 e 4 ele começa a seguir um **sentido horário**, o seja, vai do topo, até por fim, a esquerda, afetando individualmente cada um dos lados. 

## Unidades de medida

O CSS possui algumas **unidades de medida** que podem ser utilizadas como valor para **diversas propriedades**, além dos **pixels** (px), que se baseiam o que seria um "ponto" da tela de um dispositivo, e **porcentagens** (%) que se baseia do tamanho total do elemento parente, há outras 2 unidades de medida **notáveis**:

### Em

Um **em** se baseia no **font-size** do elemento parente a si, por exemplo, 2em seria o dobro do **font-size**, o que o torna especial é tornar o site mais acessível, pois permite o ajuste da fonte através do navegador, diferente do que **pixels**, onde o tamanho não é alterado. O único problema que **em** pode causar é por multiplicar com o valor da **font-size** do elemento parente, ou seja, vamos pensar que eu já estava utilizando em no elemento parente, então, o 2em que antes era o dobro do **font-size** se torna o quádruplo, e por assim vai, o que pode causar confusões e um código bagunçado, por isso, é preferível se utilizar de seu "parente"

### Rem

Um **rem** é como o **em**, porém ao invés de se basear no elemento parente a si, ele irá se basear no **elemento raiz**, ou seja, por todo o site **rem** terá o mesmo valor, diferente do que aconteceria com o **em**. Uma dica é utilizar como o **font-size** do elemento raíz, ou seja, o **html** como **62.5%**, assim, o seu **rem** irá igual a 10 pixels, o que te permite alcançar **boa parte dos números com facilidade**, apenas o dividindo por 10. Por exemplo, 16 pixels seria igual a 1.6rem. **Isso o faz ser a unidade de medida mais recomendada**.

### Vw e Vh

Ambos **vw** e **vh** são unidades de medida baseadas na tela do usuário, ou seja 1 **vw** ou **vh** vale a 1% da largura e altura da tela do usuário respectivamente. Eles são usados principalmente para criar designs responsivos. 

## Display

No CSS, **diversos elementos** possuem **diferentes tipos de display**, ou seja, eles são colocados na tela de forma diferente um do outro. Você pode modificar o **display** atual de um elemento através da propriedade de mesmo nome.

O primeiro tipo de display se chama **block**, ele permite mudanças de **width** e **height** e adição de **margin** e **padding** para todos os lados, porém, cada elemento que estiver com o display **block** irá simplesmente "guardar" toda a largura ao seu lado para si, então outros elementos não podem ficar ao seu lado, fazendo com que eles sejam colocados embaixo.

O segundo tipo de display é o **inline**, todos os elementos que estiverem com ele irão se organizar de forma ao invés de ficarem um embaixo do outro, eles ficarão **um do lado do outro**, e diferente do display **block**, ele não ocupa toda a largura ao seu lado, o que comporta outros elementos. Porém, diferentemente do display **block**, você não consegue alterar a **width** e **height**, e **padding** e **margin** ficam limitados apenas a esquerda e direita.

O terceiro tipo de display é o **inline-block**, sendo uma mistura dos 2 primeiros tipos, ele funciona como o segundo, porém sem limitações na alteração da **width**, **height**, **padding** e **margin**.

## **Position**

Junto ao **display**, há outra **propriedade** que podemos utilizar para modificar a forma com que certo elemento é colocado na tela, sendo ele o **position**. O valor inicial de position, ou seja, aquele que os elementos já tem de início é chamado **static**, onde você não consegue mudar diretamente a sua posição sem o uso de **display**, por exemplo. 

Contudo, as outras opções de position permitem que o posicionamento seja modificado diretamente, utilizando-se das propriedades **top**, **bottom**, **right** e **left**. Vale lembrar, que essas propriedades, quanto menor o valor, mais perto será, ou seja, caso o top seja 0rem, o elemento ficará exatamente no topo e por assim vai.

### Absolute

O **position: absolute** torna o elemento livre para qualquer movimentação, ou seja, ele pode "**ultrapassar**" o seu elemento parente.

### Relative

No **position: relative**, a movimentação não é completamente livre assim como no **absolute**, sendo mais preciso, ela é livre mas ela não pode ultrapassar o seu elemento parente.

### Fixed

Com o **position: fixed**, a posição é relativa a parte visível do website, ou seja, independente de você  usar a barra de rolagem, o elemento ficará sempre a mostra no mesmo "lugar" em relação a sua tela.

### Sticky

Através do **position: sticky**, quando o elemento está prestes a "sumir da tela" conforme você navega, ele se prende a tela, algo muito utilizado para fazer cabeçalhos, por exemplo.

## Pseudo-classes

Além de podemos selecionar elementos no CSS, também podemos selecionar "**estados**" desses elementos e **modificá-los** de acordo, permitindo muito mais mudanças, tudo que você precisa é colocar **:** + **pseudo-classe**, por exemplo:

```css
button:hover {
	color: blue;
	cursor: pointer;
}
```

Como mostrado no exemplo, utilizamos a **pseudo-classe** "**hover**", que é o estado de quando um elemento está com o **cursor por cima**, muito utilizado para dar um **feedback** ao usuário. Além disso, como "bônus", coloquei a propriedade **cursor** com o valor **pointer**, que demonstra que o elemento passado por cima pode ser clicado, esses são outros exemplos de pseudo-classes:

`**focus`** estado de um elemento que foi focado, muito usado para **inputs**.

`**link`**  estado de um link que não foi visitado ainda.

**`visited`** estado de um link quando clicado.

**`checked`** estado de que um elemento **radio**, **checkbox** ou **option** foi alterado.

## Media Queries

Com a chegada e popularização dos celulares e tablets, se tornou **fundamental** com que a maioria dos websites tenham suporte para **dispositivos mobile**, uma das formas de garantir esse suporte é através de **media queries**, que definem estilos de acordo com o tamanho da tela, veja esse exemplo:

```css
@media (max-width: 600px) {
	font-size: 1.3rem;
}
```

Como podemos ver, o **media query** que criamos tem como alvo dispositivos de até **600px** de largura, ou seja, podemos utilizar isso para ajustar parte do código tornando-o mais acessível para dispositivos móveis. Podemos também, fazer o inverso utilizando **min-width** ou até colocar um mínimo e máximo utilizando um **and** entre ambas as propriedades. **Vale lembrar, que a intenção é manter um código base fora de um media query, quase sempre o de desktop e adicionar media queries para tablets e celulares.**

Além disso, **media queries** podem ser **incorporados** no **HTML**, pois caso tenhamos um media query para diferentes tipos de dispositivos num mesmo **arquivo** isso pode torná-lo **bagunçado**, então podemos separar o código para cada dispositivo diferente, e depois na **head** do nosso HTML fazer o seguinte:

```css
<head>
<link rel="stylesheet" href="/desktop.css">
<link rel="stylesheet" href="/tablet.css" media="(max-width:1024px)">
<link rel="stylesheet" href="/smartphone.css" media="(max-width:600px)">
</head>
```

Assim, os estilos serão utilizados de acordo com a tela do usuário de uma forma organizada. É bom sempre **colocar acima** o **CSS** do desktop, para evitar com que ele seja sobrescrito acidentalmente.

## Flexbox

**Flexbox** apesar de ser um tipo de **display**, é muito mais do que uma **propriedade**, e por isso merece uma categoria própria. **Flexbox**, que traduzido seria algo como "**caixa flexível**" funciona como uma forma de organizar estruturas de uma forma responsiva, podendo se posicionar em qualquer direção e tendo tamanhos adaptáveis. O Flexbox possui várias propriedades adicionais, que iremos cobrir agora:

### Flex-direction

A propriedade **flex-direction**, adicionada ao **elemento-pai**, define qual será a direção que os **elementos-filho** irão seguir, seus valores são:

`**row`** valor padrão, que organiza os itens da esquerda para a direita, como uma linha.

`**row-reverse`** assim como o row, porém a ordem dos itens será invertida, começando do último elemento-filho até o primeiro.

`**column**` organiza os itens de cima para baixo, como uma coluna.

`**column-reverse**` assim como o column, porém começando do último elemento-filho e indo até o primeiro.

### Flex-wrap

A propriedade **flex-wrap**, adicionada ao **elemento-pai**, ****define como os **elementos-filho** serão realocados ou não, caso não caibam mais no espaço disponível em tela, utilizando-se desses valores:

**`nowrap`** sendo o valor original, faz com que os elementos não sejam realocados quando não caberem na tela do usuário, diminuindo o tamanho dos elementos-filhos.

**`wrap`** fará os elementos se reorganizarem para baixo ou lado quando o tamanho da tela for menor que o dos elementos.

**`wrap-reverse`** assim como o wrap, porém irá começar do último elemento-filho até o primeiro.

### Justify-content

A propriedade **justify-content**, adicionada ao **elemento-pai**, define como os **elementos-filho** serão alinhados horizontalmente (isso quando **flex-direction: row**) e verticalmente (isso quando **flex-direction: column**), esses são seus valores:

**`flex-start`** irá alinhar os elementos-filho ao começo (esquerda ou cima) do elemento-pai.

**`flex-end`**  alinhará os elementos-filho ao final (direita ou baixo) do elemento-pai.

**`center`** deixará os elementos-filho alinhados ao centro do elemento-pai.

**`space-around`** deixará os elementos-filho espaçados entre si (com um espaço menor no primeiro e último elemento)

**`space-evenly`** tornará os elementos-filho espaçados igualmente.

### Align-items

A propriedade **align-items**, adicionada ao **elemento-pai**, define como os **elementos-filho** serão alinhados verticalmente (isso quando **flex-direction: row**) e horizontalmente (isso quando **flex-direction: column**), esses são seus valores:

**`flex-start`** irá alinhar os elementos-filho ao começo (cima ou esquerda) do elemento-pai.

**`flex-end`**  alinhará os elementos-filho ao final (baixo ou direita) do elemento-pai.

**`center`** deixará os elementos-filho alinhados ao centro do elemento-pai.

**`strech`** caso os elementos-filho não tenham uma altura definida, eles serão "esticados" até cobrir o espaço inteiro do elemento-pai.

## Estilizando

Como há mais exemplos teóricos do que práticos, o que faz com que muitas coisas acabem se perdendo, essa área é feita com a intenção de compartilhar a criação de diferentes coisas como uma forma de ensinar diferentes estilizações e propriedades com o CSS e também demonstrar um uso mais práticos dos elementos semânticos do HTML. Todos estão cheios de comentários explicando o que está ocorrendo e algumas coisas extras, divirta-se:

 

- [Botão](https://codepen.io/yan-thomas/pen/rNMvOMG)
