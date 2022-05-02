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
