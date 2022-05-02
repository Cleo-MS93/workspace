#            Programação Java



#### Eclipse IDE

     O Eclipse é uma ferramenta IDE que compreende vários tipos de linguagem e que aceita a instalação de plugins para emular o desenvolvimento da plataforma.
     Uma das principais vantagens é o uso do SWT (alternativa para quem desenvolve em SWING), e a forte orientação ao desenvolvimento baseado em plugins ampliando o suporte do desenvolvedor com centenas deles que procuram atender as diferentes necessidades.

#### Perspectiva

     A perspectiva define quais e como surgem na Workbench as visões (views) que estão associadas. Essas views podemos considerar como a emulação da linguagemque vai ser trabalhada na aplicação. 
     
    Ex: Window > Perspective > Open Perspective > Java

#### Atalhos uteis Eclipse


 - CTRL + SHIFT + W:  Fechar todas as abas;

 - CTRL + O:  Localizar método / atributo em uma classe;

 - CTRL + SHIFT + R:  Localizar arquivos no workspace;

 - CTRL + SHIFT + T:  Descobrir onde estão as classes em um workspace mesmo que dentro de um jar;

 - CTRL + SHIFT + L:  Lista de atalhos do Eclipse;

 - CTRL + F6:  Navegar entre os arquivos abertos;

 - CTRL + F7:  Navegar entre as abas da perspectiva;

 - CTRL + F8:  Navegar pelas perspectivas abertas;

 - CTRL + H:  Pesquisa onde está sendo utilizado determinado método, basta
   posicionar o cursor no método desejado;

 - CTRL + SHIFT + F:  Formata o código conforme os padrões setados nas 
   preferências do eclipse;

 - CTRL + SHIFT + O:  Organiza os imports da classe;

 - CTRL + ALT + H:  Mostra todas as ocorrências de um atributo ou método dentro de uma classe;

 - ALT + SHIFT + L:  Extrai o que estiver selecionado para uma variável;

 - ALT + SHIFT + M:  Extrai o que estiver selecionado para um método;

 - CTRL + SHIFT + C:  Comentar / Descomentar um bloco de código;

 - CTRL + SHIFT + / : Comentar um grande bloco de código com /* */;

 - CTRL + SHIFT + \:  Descomentar um grande bloco de código com /* */;

 - CTRL + I:  Indenta corretamente o código conforme preferências do eclipse;

 - CTRL + SHIFT + B:  Inserir / excluir breakpoint na linha onde está o cursor;

 - CTRL + M:  Maximizar a tela de edição de código;

 - CTRL + ESPAÇO:  Autocompleta;

 - CTRL + 1:  Correções quando há erros de compilação, para novas classes, ou
   até mesmo quando precisar importar pacotes;

 - CTRL + 3:  Busca um comando ou uma opção de menu baseado no que você escreve;

      Todos os atalhos Eclipse IDE: http://www.w3big.com/pt/eclipse/eclipse-shortcuts.html

   



### Variáveis, Tipos de Dados e Operadores Matemáticos em Java



### Oque é uma Variável?

"Um espaço na memória do computador, onde se pode guardar valores"

Existem 4 tipos:

 - instancia: objeto
 - Classe: classe
 - Local: dentro de métodos
 - Parâmetro: na assinatura do método



### Criação

Padrão de definição:

<?visibilidade?> <?modificador?> tipo de nome <?=valorInicial?>;

- V: "public", "protected" e "private"

- M: "static" e "final"
- T: tipo de dado
- N: nome que é fornecido a variável
- VI: um valor inicial, caso se deseje



Convenções e regras:

- Não devem começar com números;
- Embora permitido, "$" e "_" devem ser evitados;
- São case-sensitive;
- Sem espaços;
- Não pode ser as palavras reservadas;



### Boas práticas

- Sempre começar com letra minúscula;
- Nomes expressivos;
- Notação camelo;
- Quando constante(final) maiúscula e separada por "_";

Exemplos:

- int quantidadeProduto; (Boa prática)

- ##### int QuantidadeProduto;

- int final NUMERO_TENTATIVAS = 5; (Boa prática)

- ##### int final numeroTentativas = 5;

- ##### int NUMERO_TENTATIVAS = 5;

- ##### int qtdProd;

- int i;

  É importante as boas práticas na programação sempre serem seguidas para que o código fique fácil de ser compreendido por outros desenvolvedores que forem alterar o código.



### Operadores

  Agora que você aprendeu a declarar e inicializar variáveis, provavelmente quer saber como *fazer algo* com elas. Aprender os operadores da linguagem de programação Java é um bom ponto de partida. Os operadores são símbolos especiais que realizam operações específicas em um, dois ou três *operandos* e, em seguida, retornam um resultado.

  À medida que exploramos os operadores da linguagem de programação Java, pode ser útil saber com antecedência quais operadores têm a precedência mais alta. Os operadores na tabela a seguir são listados de acordo com a ordem de precedência. Quanto mais próximo do topo da tabela um operador estiver, maior será sua precedência. Operadores com maior precedência são avaliados antes de operadores com precedência relativamente menor. Operadores na mesma linha têm a mesma precedência. Quando operadores de igual precedência aparecem na mesma expressão, uma regra deve governar qual é avaliada primeiro. Todos os operadores binários, exceto os operadores de atribuição, são avaliados da esquerda para a direita; os operadores de atribuição são avaliados da direita para a esquerda.

| Operadores             | Precedência                              |
| ---------------------- | ---------------------------------------- |
| pós-fixação            | `*expr*++ *expr*--`                      |
| unário                 | `++*expr* --*expr* +*expr* -*expr* ~ !`  |
| multiplicativo         | `* / %`                                  |
| aditivo                | `+ -`                                    |
| mudança                | `<< >> >>>`                              |
| relacional             | `< > <= >= instanceof`                   |
| igualdade              | `== !=`                                  |
| E bit a bit            | `&`                                      |
| OU exclusivo bit a bit | `^`                                      |
| OU inclusivo bit a bit | `|`                                      |
| E lógico               | `&&`                                     |
| OU lógico              | `||`                                     |
| ternário               | `? :`                                    |
| tarefa                 | `= += -= *= /= %= &= ^= |= <<= >>= >>>=` |



  Na programação de propósito geral, certos operadores tendem a aparecer com mais frequência do que outros; por exemplo, o operador de atribuição " `=`" é muito mais comum do que o operador de deslocamento à direita sem sinal " `>>>`". Com isso em mente, a discussão a seguir se concentra primeiro nos operadores que você provavelmente usará regularmente e termina focando naqueles que são menos comuns. Cada discussão é acompanhada por código de exemplo que você pode compilar e executar. Estudar sua saída ajudará a reforçar o que você acabou de aprender.



### Variáveis

Como você aprendeu na lição anterior, um objeto armazena seu estado em *campos* .

```
int cadência = 0;
int velocidade = 0;
int engrenagem = 1;
```

O [que é um objeto? ](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)discussão introduziu você aos campos, mas você provavelmente ainda tem algumas perguntas, como: Quais são as regras e convenções para nomear um campo? Além disso `int`, que outros tipos de dados existem? Os campos precisam ser inicializados quando são declarados? Os campos são atribuídos a um valor padrão se não forem inicializados explicitamente? Vamos explorar as respostas para essas perguntas nesta lição, mas antes disso, há algumas diferenças técnicas que você deve primeiro conhecer. Na linguagem de programação Java, os termos "campo" e "variável" são usados; esta é uma fonte comum de confusão entre os novos desenvolvedores, já que ambos parecem se referir à mesma coisa.

A linguagem de programação Java define os seguintes tipos de variáveis:

- **Variáveis de Instância (Campos Não Estáticos)** Tecnicamente falando, os objetos armazenam seus estados individuais em "campos não estáticos", ou seja, campos declarados sem a palavra- `static`chave. Campos não estáticos também são conhecidos como *variáveis de instância* porque seus valores são exclusivos para cada *instância* de uma classe (para cada objeto, em outras palavras); a `currentSpeed`de uma bicicleta é independente da `currentSpeed`de outra.
- **Variáveis de classe (campos estáticos)** Uma *variável de classe* é qualquer campo declarado com o `static`modificador; isso informa ao compilador que existe exatamente uma cópia dessa variável, independentemente de quantas vezes a classe foi instanciada. Um campo definindo o número de marchas para um tipo específico de bicicleta pode ser marcado como `static`desde que conceitualmente o mesmo número de marchas será aplicado a todas as instâncias. O código `static int numGears = 6;`criaria um campo estático. Além disso, a palavra-chave `final`pode ser adicionada para indicar que o número de marchas nunca mudará.
- **Variáveis Locais** Semelhante à forma como um objeto armazena seu estado em campos, um método geralmente armazena seu estado temporário em *variáveis locais* . A sintaxe para declarar uma variável local é semelhante à declaração de um campo (por exemplo, `int count = 0;`). Não há nenhuma palavra-chave especial designando uma variável como local; essa determinação vem inteiramente do local em que a variável é declarada — que fica entre as chaves de abertura e fechamento de um método. Como tal, as variáveis locais são visíveis apenas para os métodos nos quais são declaradas; eles não são acessíveis pelo resto da classe.
- **Parâmetros** Você já viu exemplos de parâmetros, tanto na `Bicycle`classe quanto no `main`método do método "Hello World!" inscrição. Lembre-se de que a assinatura do `main`método é `public static void main(String[] args)`. Aqui, a `args`variável é o parâmetro para este método. O importante a lembrar é que os parâmetros são sempre classificados como "variáveis" e não como "campos". Isso também se aplica a outras construções que aceitam parâmetros (como construtores e manipuladores de exceção) que você aprenderá mais adiante no tutorial.

Dito isso, o restante deste tutorial usa as seguintes diretrizes gerais ao discutir campos e variáveis. Se estamos falando de "campos em geral" (excluindo variáveis e parâmetros locais), podemos simplesmente dizer "campos". Se a discussão se aplicar a "todas as opções acima", podemos simplesmente dizer "variáveis". Se o contexto exigir uma distinção, usaremos termos específicos (campo estático, variáveis locais etc.) conforme apropriado. Você também pode ocasionalmente ver o termo "membro" usado também. Os campos, métodos e tipos aninhados de um tipo são chamados coletivamente de seus *membros* .



### Nomeação

Cada linguagem de programação tem seu próprio conjunto de regras e convenções para os tipos de nomes que você pode usar, e a linguagem de programação Java não é diferente. As regras e convenções para nomear suas variáveis podem ser resumidas da seguinte forma:

- Os nomes de variáveis diferenciam maiúsculas de minúsculas. O nome de uma variável pode ser qualquer identificador legal — uma sequência de comprimento ilimitado de letras e dígitos Unicode, começando com uma letra, o cifrão " `$`" ou o caractere sublinhado " `_`". A convenção, no entanto, é sempre começar seus nomes de variáveis com uma letra, não " `$`" ou " `_`". Além disso, o caractere cifrão, por convenção, nunca é usado. Você pode encontrar algumas situações em que nomes gerados automaticamente conterão o cifrão, mas seus nomes de variáveis devem sempre evitar usá-lo. Existe uma convenção semelhante para o caractere sublinhado; embora seja tecnicamente legal começar o nome da sua variável com " `_`", esta prática é desencorajada. Espaço em branco não é permitido.
- Os caracteres subsequentes podem ser letras, dígitos, cifrões ou caracteres de sublinhado. As convenções (e o bom senso) também se aplicam a essa regra. Ao escolher um nome para suas variáveis, use palavras completas em vez de abreviações enigmáticas. Isso tornará seu código mais fácil de ler e entender. Em muitos casos, isso também tornará seu código autodocumentado; os campos chamados `cadence`, `speed`e `gear`, por exemplo, são muito mais intuitivos do que as versões abreviadas, como `s`, `c`e `g`. Lembre-se também de que o nome escolhido não deve ser uma [chave ou palavra reservada].
- Se o nome escolhido consistir em apenas uma palavra, escreva essa palavra com todas as letras minúsculas. Se consistir em mais de uma palavra, coloque em maiúscula a primeira letra de cada palavra subsequente. Os nomes `gearRatio`e `currentGear`são os principais exemplos dessa convenção. Se sua variável armazena um valor constante, como `static final int NUM_GEARS = 6`, a convenção muda um pouco, colocando cada letra em maiúscula e separando as palavras subsequentes com o caractere sublinhado. Por convenção, o caractere sublinhado nunca é usado em outro lugar.



### Resumo das variáveis

A linguagem de programação Java usa "campos" e "variáveis" como parte de sua terminologia. As variáveis de instância (campos não estáticos) são exclusivas para cada instância de uma classe. Variáveis de classe (campos estáticos) são campos declarados com o `static`modificador; há exatamente uma cópia de uma variável de classe, independentemente de quantas vezes a classe foi instanciada. As variáveis locais armazenam o estado temporário dentro de um método. Parâmetros são variáveis que fornecem informações extras a um método; tanto as variáveis locais quanto os parâmetros são sempre classificados como "variáveis" (não "campos"). Ao nomear seus campos ou variáveis, existem regras e convenções que você deve (ou deve) seguir.

Os oito tipos de dados primitivos são: byte, short, int, long, float, double, boolean e char. A [`java.lang.String`](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)classe representa cadeias de caracteres. O compilador atribuirá um valor padrão razoável para campos dos tipos acima; para variáveis locais, um valor padrão nunca é atribuído. Um literal é a representação do código-fonte de um valor fixo. Uma matriz é um objeto contêiner que contém um número fixo de valores de um único tipo. O comprimento de um array é estabelecido quando o array é criado. Após a criação, seu comprimento é fixo.





### Tipos de dados primitivos

A linguagem de programação Java é estaticamente tipada, o que significa que todas as variáveis devem primeiro ser declaradas antes de poderem ser usadas. Isso envolve informar o tipo e o nome da variável, como você já viu:

```
int engrenagem = 1;
```

Fazer isso informa ao seu programa que existe um campo chamado "engrenagem", contém dados numéricos e tem um valor inicial de "1". O tipo de dado de uma variável determina os valores que ela pode conter, mais as operações que podem ser realizadas nela. Além disso `int`, a linguagem de programação Java suporta sete outros *tipos de dados primitivos* . Um tipo primitivo é predefinido pela linguagem e é nomeado por uma palavra-chave reservada. Os valores primitivos não compartilham o estado com outros valores primitivos. Os oito tipos de dados primitivos suportados pela linguagem de programação Java são:

- **byte** : O `byte`tipo de dados é um inteiro de complemento de dois de 8 bits com sinal. Tem um valor mínimo de -128 e um valor máximo de 127 (inclusive). O `byte`tipo de dados pode ser útil para economizar memória em [arrays](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/arrays.html) grandes , onde a economia de memória realmente importa. Eles também podem ser usados no lugar de `int`onde seus limites ajudam a esclarecer seu código; o fato de o alcance de uma variável ser limitado pode servir como uma forma de documentação.
- **short** : O `short`tipo de dados é um inteiro de complemento de dois de 16 bits com sinal. Tem um valor mínimo de -32.768 e um valor máximo de 32.767 (inclusive). Assim como com `byte`, as mesmas diretrizes se aplicam: você pode usar a `short`para economizar memória em arrays grandes, em situações em que a economia de memória realmente importa.
- **int** : Por padrão, o `int`tipo de dados é um inteiro de complemento de dois com sinal de 32 bits, que tem um valor mínimo de -2 31 e um valor máximo de 2 31 -1. No Java SE 8 e posterior, você pode usar o `int`tipo de dados para representar um inteiro sem sinal de 32 bits, que tem um valor mínimo de 0 e um valor máximo de 2 32 -1. Use a classe Integer para usar `int`o tipo de dados como um inteiro sem sinal. Consulte a seção As Classes de Números para obter mais informações. Métodos estáticos como `compareUnsigned`, `divideUnsigned`etc foram adicionados à [`Integer`](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html)classe para suportar as operações aritméticas para inteiros sem sinal.
- **long** : O `long`tipo de dados é um inteiro de complemento de dois de 64 bits. O longo assinado tem um valor mínimo de -2 63 e um valor máximo de 2 63 -1. No Java SE 8 e posterior, você pode usar o `long`tipo de dados para representar um comprimento de 64 bits sem sinal, que tem um valor mínimo de 0 e um valor máximo de 2 64 -1. Use esse tipo de dados quando precisar de um intervalo de valores mais amplo do que os fornecidos por `int`. A [`Long`](https://docs.oracle.com/javase/8/docs/api/java/lang/Long.html)classe também contém métodos como `compareUnsigned`, `divideUnsigned`etc para dar suporte a operações aritméticas para unsigned long.
- **float** : O `float`tipo de dados é um ponto flutuante IEEE 754 de 32 bits de precisão simples. Seu intervalo de valores está além do escopo desta discussão, mas é especificado na seção [Tipos, formatos e valores](https://docs.oracle.com/javase/specs/jls/se7/html/jls-4.html#jls-4.2.3) de ponto flutuante da Especificação de linguagem Java. Assim como nas recomendações para `byte`e `short`, use a `float`(em vez de `double`) se precisar economizar memória em grandes matrizes de números de ponto flutuante. Esse tipo de dados nunca deve ser usado para valores precisos, como moeda. Para isso, você precisará usar a classe [java.math.BigDecimal . ](https://docs.oracle.com/javase/8/docs/api/java/math/BigDecimal.html)Capas de [Numbers e Strings](https://docs.oracle.com/javase/tutorial/java/data/index.html)`BigDecimal` e outras classes úteis fornecidas pela plataforma Java.
- **double** : O `double`tipo de dados é um ponto flutuante IEEE 754 de precisão dupla de 64 bits. Seu intervalo de valores está além do escopo desta discussão, mas é especificado na seção [Tipos, formatos e valores](https://docs.oracle.com/javase/specs/jls/se7/html/jls-4.html#jls-4.2.3) de ponto flutuante da Especificação de linguagem Java. Para valores decimais, esse tipo de dados geralmente é a opção padrão. Conforme mencionado acima, esse tipo de dados nunca deve ser usado para valores precisos, como moeda.
- **boolean** : O `boolean`tipo de dados tem apenas dois valores possíveis: `true`e `false`. Use esse tipo de dados para sinalizadores simples que rastreiam condições verdadeiras/falsas. Esse tipo de dados representa um bit de informação, mas seu "tamanho" não é algo definido com precisão.
- **char** : O `char`tipo de dados é um único caractere Unicode de 16 bits. Tem um valor mínimo de `'\u0000'`(ou 0) e um valor máximo de `'\uffff'`(ou 65.535 inclusive).

Além dos oito tipos de dados primitivos listados acima, a linguagem de programação Java também fornece suporte especial para cadeias de caracteres por meio da classe [java.lang.String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html) . Colocar sua cadeia de caracteres entre aspas duplas criará automaticamente um novo `String`objeto; por exemplo, `String s = "this is a string";`. `String`os objetos são *imutáveis* , o que significa que, uma vez criados, seus valores não podem ser alterados. A `String`classe não é tecnicamente um tipo de dados primitivo, mas considerando o suporte especial dado a ela pela linguagem, você provavelmente tenderá a pensar nela como tal. Você aprenderá mais sobre a `String`classe em [Simple Data Objects]



### Valores padrão

Nem sempre é necessário atribuir um valor quando um campo é declarado. Os campos declarados, mas não inicializados, serão definidos com um padrão razoável pelo compilador. De um modo geral, esse padrão será zero ou `null`, dependendo do tipo de dados. Confiar nesses valores padrão, no entanto, geralmente é considerado um estilo de programação ruim.

O gráfico a seguir resume os valores padrão para os tipos de dados acima.

| **Tipo de dados**           | **Valor padrão (para campos)** |
| --------------------------- | ------------------------------ |
| byte                        | 0                              |
| baixo                       | 0                              |
| int                         | 0                              |
| grandes                     | 0L                             |
| flutuador                   | 0,0f                           |
| Duplo                       | 0,0d                           |
| Caracteres                  | '\u0000'                       |
| String (ou qualquer objeto) | nulo                           |
| boleano                     | falso                          |



As variáveis locais são ligeiramente diferentes; o compilador nunca atribui um valor padrão a uma variável local não inicializada. Se você não puder inicializar sua variável local onde ela foi declarada, certifique-se de atribuir um valor a ela antes de tentar usá-la. Acessar uma variável local não inicializada resultará em um erro em tempo de compilação.



### Literais

Você deve ter notado que a `new`palavra-chave não é usada ao inicializar uma variável de um tipo primitivo. Tipos primitivos são tipos de dados especiais embutidos na linguagem; eles não são objetos criados a partir de uma classe. Um *literal* é a representação do código-fonte de um valor fixo; literais são representados diretamente em seu código sem exigir computação. Conforme mostrado abaixo, é possível atribuir um literal a uma variável de um tipo primitivo:

```
resultado booleano = true;
char maiúsculoC = 'C';
byte b = 100;
s curto = 10.000;
int = 100.000;
```



#### Literais inteiros

Um literal inteiro é do tipo `long`se terminar com a letra `L`ou `l`; caso contrário, é do tipo `int`. É recomendado que você use a letra maiúscula `L`porque a letra minúscula `l`é difícil de distinguir do dígito `1`.

Os valores dos tipos integrais `byte`, `short`, `int`e `long`podem ser criados a partir de `int`literais. Valores de tipo `long`que excedem o intervalo de `int`podem ser criados a partir de `long`literais. Literais inteiros podem ser expressos por estes sistemas numéricos:

- Decimal: Base 10, cujos dígitos são os números de 0 a 9; este é o sistema numérico que você usa todos os dias
- Hexadecimal: Base 16, cujos dígitos consistem nos números de 0 a 9 e nas letras A a F
- Binário: Base 2, cujos dígitos consistem nos números 0 e 1 (você pode criar literais binários em Java SE 7 e posterior)

Para programação de propósito geral, o sistema decimal provavelmente será o único sistema numérico que você usará. No entanto, se você precisar usar outro sistema de numeração, o exemplo a seguir mostra a sintaxe correta. O prefixo `0x`indica hexadecimal e `0b`indica binário:

```
// O número 26, em decimal
int decVal = 26;
// O número 26, em hexadecimal
int hexVal = 0x1a;
// O número 26, em binário
int binVal = 0b11010;
```



#### Literais de ponto flutuante

Um literal de ponto flutuante é do tipo `float`se terminar com a letra `F`ou `f`; caso contrário, seu tipo é `double`e, opcionalmente, pode terminar com a letra `D`ou `d`.

Os tipos de ponto flutuante ( `float`e `double`) também podem ser expressos usando E ou e (para notação científica), F ou f (literal flutuante de 32 bits) e D ou d (literal duplo de 64 bits; este é o padrão e por convenção é omitido).

```
duplo d1 = 123,4;
// mesmo valor de d1, mas em notação científica
duplo d2 = 1,234e2;
flutuante f1 = 123,4f;
```



#### Literais de caracteres e strings

Literais de tipos `char`e `String`podem conter quaisquer caracteres Unicode (UTF-16). Se seu editor e sistema de arquivos permitirem, você poderá usar esses caracteres diretamente em seu código. Caso contrário, você pode usar um "escape Unicode" como `'\u0108'`(C maiúsculo com circunflexo) ou `"S\u00ED Se\u00F1or"`(Sí Señor em espanhol). Sempre use 'aspas simples' para `char`literais e "aspas duplas" para `String`literais. As sequências de escape Unicode podem ser usadas em outro lugar em um programa (como em nomes de campo, por exemplo), não apenas em `char`ou `String`literais.

A linguagem de programação Java também suporta algumas sequências de escape especiais para `char`e `String`literais: `\b`(backspace), `\t`(tab), `\n`(line feed), `\f`(form feed), `\r`(carriage return), `\"`(aspas duplas), `\'`(aspas simples) e `\\`( barra invertida).

Há também um `null`literal especial que pode ser usado como valor para qualquer tipo de referência. `null`pode ser atribuído a qualquer variável, exceto variáveis de tipos primitivos. Há pouco que você possa fazer com um `null`valor além de testar sua presença. Portanto, `null`é frequentemente usado em programas como um marcador para indicar que algum objeto está indisponível.

Finalmente, há também um tipo especial de literal chamado literal de *classe* , formado por um nome de tipo e acrescentando " `.class"`; por exemplo, `String.class`. Isso se refere ao objeto (de type `Class`) que representa o próprio tipo.



### Usando caracteres sublinhados em literais numéricos

No Java SE 7 e posterior, qualquer número de caracteres de sublinhado ( `_`) pode aparecer em qualquer lugar entre dígitos em um literal numérico. Esse recurso permite que você, por exemplo. para separar grupos de dígitos em literais numéricos, o que pode melhorar a legibilidade do seu código.

Por exemplo, se o seu código contém números com muitos dígitos, você pode usar um caractere de sublinhado para separar os dígitos em grupos de três, da mesma forma que usaria um sinal de pontuação como uma vírgula ou um espaço como separador.

O exemplo a seguir mostra outras maneiras de usar o sublinhado em literais numéricos:

```
longo creditCardNumber = 1234_5678_9012_3456L;
long socialSecurityNumber = 999_99_9999L;
flutuante pi = 3,14_15F;
hexBytes longos = 0xFF_EC_DE_5E;
palavras hexadecimais longas = 0xCAFE_BABE;
long maxLong = 0x7fff_ffff_ffff_ffffL;
bytes nybbles = 0b0010_0101;
bytes longos = 0b11010010_01101001_10010100_10010010;
```

Você pode colocar sublinhados apenas entre dígitos; você não pode colocar sublinhados nos seguintes locais:

- No início ou no final de um número
- Adjacente a um ponto decimal em um literal de ponto flutuante
- Antes de um `F`ou `L`sufixo
- Em posições onde se espera uma sequência de dígitos

Os exemplos a seguir demonstram posicionamentos de sublinhado válidos e inválidos (que são destacados) em literais numéricos:

```
// Inválido: não pode colocar sublinhados 
// adjacente a um ponto decimal
float pi1 = 3_.1415F;
// Inválido: não pode colocar sublinhados  
// adjacente a um ponto decimal
flutuar pi2 = 3._1415F;
// Inválido: não pode colocar sublinhados  
// antes de um sufixo L
longo socialSecurityNumber1 = 999_99_9999_L;

// OK (literal decimal)
int x1 = 5_2;
// Inválido: não pode colocar sublinhados 
// No final de um literal
int x2 = 52_;
// OK (literal decimal)
int x3 = 5_______2;

// Inválido: não é possível colocar sublinhados 
// no prefixo de raiz 0x
int x4 = 0_x52;
// Inválido: não pode colocar sublinhados 
// no início de um número
int x5 = 0x_52;
// OK (literal hexadecimal)
int x6 = 0x5_2;
// Inválido: não pode colocar sublinhados 
// no final de um número
int x7 = 0x52_;
```



