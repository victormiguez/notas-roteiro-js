### Notas do Roteiro ["Como Aprender JavaScript Corretamente"](https://groups.google.com/forum/#!forum/impjs---grupo-01-roteiro-como-aprender-javascript-corretamente)

#### O que serão estas notas?

Um local para sintetizar o conteúdo aprendido e auxiliar os colegas que irão começar a estudar por este roteiro também. As notas irão conter os tópicos abordados pelo livro *"Professional JavaScript for WebDevelopers"* de Nicholas C. Zakas, porém os materiais utilizados para os estudos serão variados. 

**OBS: Todos os materiais aqui usados serão gratuitos, capítulos de amostra ou livros já adquiridos.** 

Ao longo dos tópicos, deixarei um resumo sobre o mesmo, criarei exemplos e também deixarei indicada a bibliografia utilizada para cada parte. Ao término do roteiro, irei tentar compilar todo este material criado pelas notas e gerar um livro, para treinar essa parte que tenho muito interesse em trabalhar. 

Tanto este material como o livro serão **gratuitos** para a comunidade. 

#### por [eo_op](https://github.com/eoop/eo_op)

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/br/deed.pt_BR"><img alt="Licença Creative Commons" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/br/88x31.png" /></a><br />Este obra foi licenciado sob uma Licença <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/br/deed.pt_BR">Creative Commons Atribuição-NãoComercial-CompartilhaIgual 3.0 Brasil</a>.

---

# Índice

### Semana 1 e 2

**1) O que é JavaScript?**

* [Uma breve História](#uma-breve-hist%C3%B3ria)
* [Implementações do JavaScript](#implementa%C3%A7%C3%B5es-do-javascript)
	* [ECMAScript](#ecmascript-)
	* [Document Object Model - DOM](#document-object-model---dom-)
	* [Browser Object Model - BOM](#browser-object-model---bom-)
	* [Exemplos de uso - DOM e BOM](#exemplos-de-uso---dom-e-bom-)

---

# Semana 1 e 2 [⇪](#%C3%8Dndice)

## 1) O que é JavaScript? [⇪](#%C3%8Dndice)

### Uma breve História [⇪](#%C3%8Dndice)

O JavaScript nasceu para suprir uma carência deixada quando os applets Java™ falharam como "linguagem oficial da internet". Então, em 1996, foi introduzido ao Netscape Navigator 2 o JavaScript pela primeira vez, mesmo de forma ainda um pouco "bruta". A internet estava engatinhando, então a qualidade do código não era algo exigido, fazendo com que a linguagem por muito tempo tenha ficado mal vista perante os programadores.

A missão do JavaScript era economizar tempo. Nos primórdios, a internet era bastante lenta e as requisições feitas ao servidor demandavam um longo tempo de espera para o envio e carregamento da informação esperada. Sendo assim, o JavaScript, por exemplo, fazia a verificação dos dados de um formulário antes que o mesmo fosse enviado ao servidor, para evitar que se algo de cara não estivesse correto, o usuário seria informado de imediato, economizando assim um bom tempo.

Aliado a isso, o JavaScript é também responsável por manipular os elementos da página, vitalizando toda a estrutura criado pelo HTML. E não para por aí, além de funcionar no lado do cliente, o JavaScript está cada vez mais ganhando espaço e sendo utilizados em diversas plataformas. No lado do servidor, temos o .NET e o Node.JS, nos sistemas operacionas as aplicações desktop (rodando em diversos sistemas), criando aplicativos para dispositivos móveis e também criando extensões para navegadores (chrome e firefox por exemplo) e também programas como o Photoshop.

Temos várias outras peculiaridades na linguagem JavaScript, que ao decorrer desta viagem nós iremos descobrir... 

> **fonte:** JavaScript de Alto Desempenho - Nicholas C. Zakas | Padrões JavaScript - Stoyan Stefanov

### Implementações do JavaScript [⇪](#%C3%8Dndice)

Apesar de serem postos como sinônimos, o JavaScript e o ECMAScript não possuem tal relação pois como podemos observar na ilustração abaixo, o JavaScript é a junção do ECMAScript (no caso o núcleo), o DOM (Document Objetc Model) e o BOM (Browser Object Model).

![js-ecma-dom-bom](http://i.imgur.com/78YVXKG.png)

### ECMAScript [⇪](#%C3%8Dndice)

É uma linguagem de script que não é ligada somente aos navegadores. Ela forma a base do JavaScript, e foi padronizada pela organização [Ecma International](http://www.ecma-international.org/) na especificação **ECMA- e ECMA-402.**

Cuida basicamente das seguintes partes da linguagem:

* Sintaxe
* Tipos
* Statements (afirmações)
* Palavras-chave
* Palavras reservadas
* Operadores
* Objetos

### Document Object Model - DOM [⇪](#%C3%8Dndice)

O Modelo de Objeto de Documentos (DOM) é uma API (Application Programming Interface - Interface de Programação de Aplicativos) criada para que nós possamos alterar e editar a estrutura, conteúdo e estilo de um documento eletrônico, independente da plataforma e da linguagem. A API DOM fornece uma maneira padrão de acesso aos elementos contidos no documento, além de permitir o trabalho com os mesmos de forma isolada, possibilitando a criação de páginas altamente dinâmicas. 

O DOM mapeia toda a página como um documento composto de nós hierárquicos como uma estrutura de árvore e usa a DOM API, os nós podem ser removidos, adicionados e substituídos. São dividos em 3 níveis:

**DOM nível 1**: tem 2 módulos. O *DOM Core* fornece o caminho para mapear a estrutura documento para fácil acesso e manipulação. *DOM HTML*, extende o DOM Core adicionando objetos e métodos específicos para o HTML.

**DOM nível 2**: introduziu diversos novos módulos DOM para lidar com novos tipos de interfaces:

* DOM Views - descreve interfaces para acompanhar as várias views de um documento (ou sejna, o documento antes do estilo CSS e depois do estilo CSS)
* DOM Events - descreve interfaces para eventos
* DOM Style - descreve interfaces para lidar com estilos baseados no CSS
* DOM Traversal and Range - descreve interfaces para percorrer e manipular um árvore de documento

**DOM nível 3:** amplia ainda mais o DOM com a introdução de métodos para carregar e salvar documentos de forma uniforme (contendo um novo módulo chamado 'DOM Load and Save'), como também métodos para validar o documento (DOM Validation).

Note que o DOM não é específico ao JavaScript, e de fato tem sido implantado em inúmeras outras linguagens. Para navegadores, entretanto, o DOM foi implementado usando ECMAScript e agora torna-se uma grande parte da linguagem JavaScript.

**Outros DOMs**

* Scalable Vector Graphics (SVG)
* Mathematical Markup Language (MathML)
* Synchronized Multimedia Integration Language (SMIL)

### Browser Object Model - BOM [⇪](#%C3%8Dndice)

O BOM (Modelo de Objeto do Navegador) permite o acesso e a manipulação da janela do navegador, podendo assim interagir com o navegador em um contexto fora do mostrado na página. Um problema notado no BOM é o fato de não haver uma padronização. O HTML5 cuidou de boa parte desta especificação, nos livrando de muitos problemas causados pelo BOM.

Vamos ver algumas propriedades do BOM: 

> Trecho extraído do livro Professional JavaScript for WebDevelopers - Nicholas C. Zakas (seção disponibilizada [aqui](http://www.amazon.com/Professional-JavaScript-Developers-Nicholas-Zakas/dp/1118026691))

* Capacidade de criar novas janelas no navegador
* Capacidade de mover, redimensionar e fechar janelas do navegador
* O objeto `navigator`, que fornece informações detalhadas sobre o navegador
* O objeto `location`, que nos dá informações detalhadas sobre a página carregada no navegador
* O objeto `screen`, que nos dá informações detalhadas sobre a resolução da tela do usuário
* Suporte aos cookies
* Objetos personalizados como o `XMLHttpRequest` e no Internet Explorer `ActiveXObject`

**OBS:** Podemos chamar os métodos BOM sem usar `window.nomeDaPropriedade`, pois o escopo global já está no namespace `window`.

> **Fonte:** Professional JavaScript for WebDevelopers - Nicholas C. Zakas | [Mozilla Developers Network](https://developer.mozilla.org/en-US/) | [Artigo 1](http://vkanakaraj.wordpress.com/2009/12/18/javascript-vs-dom-vs-bom-relationship-explained/)

### Exemplos de uso - DOM e BOM [⇪](#%C3%8Dndice)

##### Exemplos BOM

**window.close ()** - fecha a página atual

``` 
// teste no chrome developer tools - fecha a página atual
window.close ();

```

**window.history** - Manipula os enventos relacionados ao histórico da página.

Exemplo de uma propriedade:

**window.history.length**: retorna o número inteiro representando o número de páginas no histórico de sessão, incluindo a página atual carregada. Se for a primeira página aberta, por exemplo, o valor retornado será 1.

```
// teste no chrome developer tools
history.length

```
exemplo no [jsFiddle](http://jsfiddle.net/3cBys/)

Exemplo de um método:

**window.history.back ()** - BOM: Carrega a página anterior a atual.

``` 

// teste no chrome developer tools
history.back ();

```
**exemplo no [jsFiddle](http://jsfiddle.net/UmSk9/2/)**

Veja também o exemplo do método `go()`. **[jsFiddle](http://jsfiddle.net/TeKuV/5/)**


##### Exemplos DOM

// em breve


> Material de Referência bem completo: [BOM](https://developer.mozilla.org/en-US/docs/Web/API/Window) e [DOM](https://developer.mozilla.org/en-US/docs/DOM/DOM_Reference)


