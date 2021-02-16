## Sobre o repositório e como colaborar

Criei esse e (irei criar outros) repositórios no GitHub com a intenção de compartilhar meus aprendizados, servindo quase que como uma mini-documentação da tecnologia em questão. 

Sinta-se livre para abrir **issues** caso encontre qualquer tipo de erro, seja de escrita, alguma informação incorreta/incompleta, etc, informando aonde está o erro e a correção ou uma sugestão de correção.

Estarei escrevendo quase que diariamente melhorias e adições ao repositório, lembrando que minha intenção é criar um repositório que se aprofundará com o tempo, não viso recriar completamente a documentação do HTML (ou outra tecnologia) em português. 

Como maior fonte de informação, utilizei os tutoriais e documentação da [W3Schools](https://www.w3schools.com/), a qual citarei de vez em quando. Acredito que **juntos** podemos criar um ótimo repositório para que desenvolvedores possam se aperfeiçoar, conferir ou aprender coisas novas!



# HTML

**HTML** significa **Hyper Text Markup Language** (Linguagem de Marcação de Hipertexto), tendo sido inicialmente lançado em 1993, sendo sua versão mais recente o HTML5 (versão 5), a qual este repositório se baseia, sendo a linguagem padrão para a criação de websites como a estrutura do seu conteúdo atualmente. 

O **HTML** funciona a partir de "blocos", que podem ser auto-contidos, esses que eu chamarei de tags, ou que precisam de uma tag de abertura e fechamento com algum conteúdo inserido, que chamarei de elementos.



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

**`<head></head>`** informações sobre o seu site, que são acessadas por mecanismos de busca e o navegador e não são visíveis ao usuário final. Geralmente a conexão com arquivos **CSS** e **JS** são feitos dentro da mesma.

**`<meta>`** inclui informações principalmente acessadas pelos mecanismos de busca, tornando o seu site mais visível.

**`<title></title>`** adicionado dentro da sua **head**, o texto que estiver inserido como conteúdo se tornará o título de sua página, que aparece na parte superior do navegador.

**`<link rel="" href="">`** faz a conexão entre dois documentos, o atributo **rel** significa relationship, basicamente pergunta o que é o arquivo que estamos conectando, por exemplo, quando for um arquivo **CSS**, utilizamos **stylesheet**, ou quando for um ícone que aparecerá em cima da página, **icon**. Já o **href**, é onde especificamos o caminho (local) do que queremos conectar.

**`<body></body>`** elemento que englobará todo o conteúdo visível ao usuário da sua página.



**Atributos importantes da tag meta:**

A tag **meta** é **importantíssima**, pois é nela onde são feitas alguns ajustes para tornar o website mais acessível a usuários de dispositivos móveis e é feita a otimização para mecanismos de busca, famosamente conhecido como **SEO**, vulgo **Search Engine Optimization ( Otimização para Mecanismos de Busca)**.
```html
//adiciona uma descrição ao seu site que é vista nos mecanismos de busca.
<meta name="description" content="A maior pizzaria à moda alemã do mundo! Pizzas a partir de R$13,99">

//especifica o charset (conjunto de caracteres) que será utilizado no site, é recomendado utilizar-se utf-8.
<meta charset="utf-8">

//define o comportamento de enquadramento da sua página, fazendo o seu website mais acessível para dispositivos móveis.
<meta name="viewport" content="width=device-width, initial-scale=1">

//determina um comportamento para os sistemas de busca ao acessarem o seu site, nesse caso, para indexar a página e seus links.
<meta name="robots" content="index, follow">

//atribui palavras-chave para mecanismos de busca indexarem sua página.
<meta name="keywords" content="pizza barata, alemã, alê pizzaria">
```




### Títulos, Parágrafos e Extras

O HTML tem elementos específicos para títulos e parágrafos, os famosos **h** e **p**.



#### Títulos

Os títulos são utilizadas principalmente para gerar hierarquia de importância, logo nem sempre o seu uso será recomendado para ter textos maiores ou em negrito, utilize **CSS** para isso, caso a maior parte do seu texto já for maior, por exemplo. Os títulos são através dos elementos **h**, de 1 à 6. **Os elementos h geram certo espaçamento próprio, como demonstrado abaixo:**



<h1>Título H1</h1>

```html
<h1>Título H1</h1>
```

<h2>Título H2</h2>

```html
<h2>Título H2</h2>
```

<h3>Título H3</h3>

```html
<h3>Título H3</h3>
```

<h4>Título H4</h4>

```html
<h4>Título H4</h4>
```

<h5>Título H5</h5>

```html
<h5>Título H5</h5>
```

<h6>Título H6</h6>

```html
<h6>Título H6</h6>
```



#### Parágrafos e Extras

No HTML você pode inserir parágrafos através do elemento **p**, além disso, você pode atribuir algumas formatações extras com outros elementos.

```html
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
```


**`<b></b>`** transforma o texto inserido em negrito.

**`<strong></strong>`** além de transformar em negrito, tem um tamanho extra. 

**`<i></i>`** deixa o texto inserido em itálico.

**`<em></em>`** além de deixar em itálico, tem um tamanho extra.

**`<mark></mark>`** deixa o texto marcado.

**`<small></small>`** deixa o texto pequeno.

**`<del></del>`** torna o texto riscado.

**`<ins></ins>`** sublinha o texto.

**`<sub></sub>`** o texto se torna subscrito.

**`<sup></sup>`** o texto se torna sobrescrito.



**Exemplo:**

```html
<p>
<strong>Bem-vindo à Alê Pizzas!</strong>
Temos uma grande variedade de <ins><b><i>pizzas alemãs</b></i></ins> com um preço mais do que <mark>saboroso!</mark>
</p>

```

**Resultado final:**

<p>
<strong>Bem-vindo à Alê Pizzas!</strong>
Temos uma grande variedade de <ins><b><i>pizzas alemãs</b></i></ins> com um preço mais do que <mark>saboroso</mark>!
</p> 




### Imagens e Vídeos



#### Imagens
Imagens são uma parte fundamental de vários websites, e podem ser facilmente inseridos no seu documento HTML, como demonstrado abaixo com a tag **img**:

```html
<img src="/pizza.jpg" alt="Pizza de mussarela">
```

O atributo **src** é onde você colocará o caminho de sua imagem, e o **alt** é tão importante quanto, pois serve como uma descrição do que é aquela imagem, que permite usuários de leitores de tela entenderem as imagens, tornando o site mais acessível. **O uso do atributo 'alt' é considerado uma boa prática.** Também pode ser inserido uma altura e largura fixa à imagem através dos atributos **width** (largura) e **height** (altura) utilizando-se pixels como medida.
&nbsp;


#### Vídeos
Vídeos, assim como imagens, podem ser inclusos em um website com uma enorme facilidade através do elemento **video**, além de algumas funcionalidades extras para melhorarem a experiência. A síntaxe para a mesma é simples:

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

Foi adicionado um pequeno texto de erro no final da tag **video**, que é mostrado apenas quando nenhuma das fontes dos vídeos funciona. Também há a adição do atributo **type**, para especificar o formato do vídeo, sempre seguindo o padrão **video/[extensão do arquivo de vídeo]**. As fontes dos vídeos serão utilizadas de acordo com a ordem, ou seja, apenas há chance da segunda fonte ser mostrada caso a primeira não funcione, assim por diante.






### Links e Âncoras
Algo de muita importância também são os links, que conectam diferentes páginas, ou diferentes partes de uma página de forma bem intuitiva através do elemento **a**:

```html
<a href="https://www.w3schools.com/tags/tag_a.asp" target="_blank">Veja mais sobre a tag a</a>
```
Através do atributo **href** você colocará o link de destino, e com o atributo **target** você irá indicar um comportamento, no caso, quando o atributo estiver ausente, ele abrirá na mesma aba, mas como temos **_blank** como valor, ele irá abrir em uma nova aba. 

Vale lembrar que o elemento **a** pode ser combinada com outras coisas, por exemplo, pode-se utilizar emojis e até outros elementos **HTML**. Olhe só, clique nesse emoji: <a href="https://emojipedia.org/" target="_blank">😀</a>


Apesar do elemento **a** ser muito útil como uma forma de disponibilizar links mais fácil e agradavelmente, isso não reflete todo seu potencial, que pode ser alcançado utilizando o elemento **a** para o propósito de seu nome: uma âncora. Uma âncora conecta duas partes da mesma página, como no exemplo abaixo:

```html
<p id="#empresa">Sobre a empresa</p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
<p>Funcinários</p>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
<a href="#empresa">Volte as informações da empresa</a>
```
O **id** é um atributo que serve para identificar exclusivamente um elemento/tag do documento e assim o acessar posteriormente, por exemplo, através de **JavaScript** ou como no exemplo dado, para criar uma âncora, ou seja, é um **href** válido, então quando clicado, a sua página automaticamente irá para a localização em questão, tornando a navegação mais intuitiva.
&nbsp;

### Formulários

Outra das funcionalidades básicas e fundamentais do **HTML** são os formulários, que te permitem lidar com a inserção de informações por parte do usuário e o envio das mesmas, sendo essa segunda parte deixada de lado por aqui, já que dependeria de uma linguagem como **PHP** ou **JavaScript** para ser melhor explicada, mas a título de curiosidade, pesquise sobre o atributo **action** adicionado no elemento **form**. A seguir, utilizarei esse código como um exemplo:
```html
//código espaçado para melhorar a clareza
<form>
    <h4>Registre-se</h4>
    <label for="username">Nome de usuário</label><br>
    <input name="username" type="text" id="username" placeholder="Insira seu nome"/>

    <br>

    <label for="useremail">E-mail</label><br>
    <input name="useremail" type="email" id="useremail" placeholder="Insira seu e-mail"/>

    <br>

    <label for="userpassword">Senha</label><br>
    <input name="userpassword" type="password" id="userpassword" placeholder="Insira uma senha forte"/>

    <br>

    <button type="submit">Finalizar cadastro</button>
</form>
```



**Resultado final:**

<form>
    <h4>Registre-se</h4>
    <label for="username">Nome de usuário</label><br>
    <input name="username" type="text" id="username" placeholder="Insira seu nome" required/>
    <br>
    <label for="useremail">E-mail</label><br>
    <input name="useremail" type="email" id="useremail" placeholder="Insira seu e-mail" required/>
    <br>
    <label for="userpassword">Senha</label><br>
    <input name="userpassword" type="password" id="userpassword" placeholder="Insira uma senha forte" required/>
    <br><br>
    <button type="submit">Finalizar cadastro</button>
</form>
&nbsp;


Como visto, vários novos elementos e tags foram apresentados, além de atributos, o que fará essa sessão um pouquinho longa (irei explicando por partes).

O elemento **form** serve como um enquadramento de todas as entradas de informação de um formulário específico, ou seja, para a sua tela de login utilizaria-se um **form**, e para a de registro, outra, e por assim vai. Bom, pode-se fazer uma analogia bem simples de que cada **form** que você inserir será uma pesquisa diferente. No **form** também pode-se adicionar o atributo **autocomplete**, onde você pode definir se o seu formulário vai auto-completar informações armazenadas no navegador do usuário ou não, através dos valores **on** e **off**, respectivamente. O atributo **autocomplete** também pode ser adicionado nos **inputs** - que irei explicar logo embaixo - individualmente, controlando mais precisamente seu comportamento.

Também foi apresentado a tag **br**, que simplesmente gera uma quebra de linha, para que o formulário não ficasse muito visualmente confuso sem o uso de **CSS**.
&nbsp;


**Label**

O elemento **label**, geralmente traduzido como rótulo ou legenda, exerce uma simples funcionalidade de especificar que tipo de **input** é preciso, ou seja a informação que é necessária. O atributo **for** serve para conectar o **id** de uma entrada com o seu devido rótulo, conexão esta que pode ser facilmente visualizada no momento em que você clica no rótulo, por exemplo, "E-mail", o **input** que estava conectado com ele através do **for** e do **id** é selecionado.
&nbsp;

**Input**

O **input** é sem dúvidas a tag mais utilizada entre os tipos de formulário, sendo acompanhado de um atributo **name**, que garante que essa informação seja enviada posteriormente de forma identificável (ou seja, será mais fácil tratar essa informação depois no seu **back-end**). Também geralmente se acompanha de um atributo **id** para colocar-se sua identificação e se conectar com sua **label**.

O atributo **type** é muito importante, pois permite vários tipos de verificações sem a necessidade de utilizar outras linguagens para isso. Como por exemplo, caso o valor do atributo seja **email**, é necessário um @ na informação digitada pelo usuário para ser válido, se não, quando o  usuário clicar para submeter o formulário, vai indicar o problema e o mesmo não será realmente enviado, ou no caso do valor ser **password**, o texto será escondido, para evitar que outras pessoas simplesmente vejam a senha enquanto você a escreve, apesar de não proteger a senha de ser descoberta. Fortemente recomendo a leitura da página sobre os diferentes tipos de **type** para o elemento **input** na [W3Schools](https://www.w3schools.com/html/html_form_input_types.asp). 

É muito bom saber também sobre o atributo **required**, pois nele é possível definir se um campo é obrigatório ou não. Ou seja, caso o campo seja obrigatório e não seja preenchido, o mesmo não será enviado, e demonstrará uma mensagem de erro.

Caso você tenha requisitos extras sobre o tamanho de um certo campo, como uma senha, você pode aproveitar-se dos atributos **minLength** e **maxLength** que recebem como valor um número que especifica a quantidade de caracteres de mínimo e máximo, respectivamente.  

&nbsp;

**Button**

O elemento **button** é simples, gera um botão clicável que executa uma função quando o mesmo é executado, tal função pode ser definida através de um valor para o atributo **type**, como por exemplo o valor **submit**, que envia as informações do formulário em que o mesmo está inserido. 

Também é possível executar **JavaScript** usando eventos como **atributos** e um pedaço de código **JavaScript** como valor desse atributo. Veja mais sobre esses eventos na [W3Schools](https://www.w3schools.com/tags/ref_eventattributes.asp).
&nbsp;


**Dropdown: Select e Option**

Utilizando-se dos elementos **select** e **option** é possível fazer uma **dropdown**, que seria como selecionar uma opção de uma lista, muito comummente utilizado no ramo dos formulários, tendo uma síntaxe bem simples:

```html
<select name="culinariafavorita" id="culinariafavorita">
    <option value="francesa">Culinária Francesa</option>
    <option value="chinesa">Culinária Chinesa</option>
    <option value="indiana">Culinária Indiana</option>
    <option value="italiana">Culinária Italiana</option>
    <option value="turca">Culinária Turca</option>
</select>
```
**Resultado final:**
<select name="culinariafavorita" id="culinariafavorita">
    <option value="francesa">Culinária Francesa</option>
    <option value="chinesa">Culinária Chinesa</option>
    <option value="indiana">Culinária Indiana</option>
    <option value="italiana">Culinária Italiana</option>
    <option value="turca">Culinária Turca</option>
</select>
&nbsp;

O atributo **select** especifica que estamos falando de um **dropdown**, aceitando dentro de si quantos elementos **option** quiser, que vem acompanhado de um atributo **value**, que diz qual será o valor dessa escolha no back-end quando o formulário for enviado, pois o texto entre as tags serve apenas na questão visual.
&nbsp;

**Textarea**

Um elemento bem simples de se explicar e que também é bem útil é o **textarea**, que cria algo semelhante a um input, porém, com a intenção de se comportar textos maiores, como por exemplo uma crítica ou como parte de uma pesquisa, como demonstrado abaixo:

```html
<textarea name="critica" id="critica" cols="30" rows="10"></textarea>
```

**Resultado final:**

<textarea name="critica" id="critica" cols="30" rows="10"></textarea>
&nbsp;

Sem muitos segredos, é assim que o **textarea** funciona. Como pode ter notado, os atributos **cols** e **rows** são novos, e com eles você pode definir o tamanho em colunas e linhas, respectivamente, fazendo seu **textarea** ter o tamanho que melhor se adequa à situação.



### Listas

Com o HTML há também a possibilidade de se criar múltiplas **listas**, **ordenadas** ou **desordenadas**, que pode ser feita facilmente, utilizando a tag **ul** ou **ol** respectivamente. Essas tags englobam uma certa quantidade de tags **li**, que são os itens da lista, como nesse exemplo:

<ol>
    <li>Maça</li>
	<li>Banana</li>
	<li>Laranja</li>
</ol>

Esse exemplo utilizou uma **ol**, no caso de uma **ul** os itens da lista seriam adicionados com uma pequena bolinha preta ao lado, que pode ser modificada utilizando **CSS**. Inclusive, você pode utilizar outras **ol** ou **ul** dentro de uma, ou adicionar outros elementos na tag **li**, muito comumente combinando-se os elementos **li** e **a** para se criar algo como um header de navegação.



### Tabelas

Tabelas, como aquelas que você encontra no Excel podem ser criadas também no HTML, com o uso dos elementos **table** - que engloba todos os outros itens de uma tabela -, **tr**, - que cria uma linha de células -, **th** - que indica o cabeçalho de uma coluna da tabela - e **td** - que seria uma célula de dados comum -.

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

O que foi escrito em **th** sempre ficará centralizado e em negrito, já o que for escrito em **td** estará sempre orientado a esquerda por padrão.



