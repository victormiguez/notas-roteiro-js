### Notas do Roteiro "Como Aprender JavaScript Corretamente"

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
	* [ECMAScript](#ecmascript)
	* [Document Object Model - DOM](#)
	* [Browser Object Model - BOM](#)
* [Versões JavaScript](#)

---

# Semana 1 e 2 [◮](#%C3%8Dndice)

## 1) O que é JavaScript? [◮](#%C3%8Dndice)

### Uma breve História [◮](#%C3%8Dndice)

O JavaScript nasceu para suprir uma carência deixada quando os applets Java™ falharam como "linguagem oficial da internet". Então, em 1996, foi introduzido ao Netscape Navigator 2 o JavaScript pela primeira vez, mesmo de forma ainda um pouco "bruta". A internet estava engatinhando, então a qualidade do código não era algo exigido, fazendo com que a linguagem por muito tempo tenha ficado mal vista perante os programadores.

A missão do JavaScript era economizar tempo. Nos primórdios, a internet era bastante lenta e as requisições feitas ao servidor demandavam um longo tempo de espera para o envio e carregamento da informação esperada. Sendo assim, o JavaScript, por exemplo, fazia a verificação dos dados de um formulário antes que o mesmo fosse enviado ao servidor, para evitar que se algo de cara não estivesse correto, o usuário seria informado de imediato, economizando assim um bom tempo.

Aliado a isso, o JavaScript é também responsável por manipular os elementos da página, vitalizando toda a estrutura criado pelo HTML. E não para por aí, além de funcionar no lado do cliente, o JavaScript está cada vez mais ganhando espaço e sendo utilizados em diversas plataformas. No lado do servidor, temos o .NET e o Node.JS, nos sistemas operacionas as aplicações desktop (rodando em diversos sistemas), criando aplicativos para dispositivos móveis e também criando extensões para navegadores (chrome e firefox por exemplo) e também programas como o Photoshop.

Temos várias outras peculiaridades na linguagem JavaScript, que ao decorrer desta viagem nós iremos descobrir... 

> **fonte:** JavaScript de Alto Desempenho - Nicholas C. Zakas | Padrões JavaScript - Stoyan Stefanov

### Implementações do JavaScript [◮](#%C3%8Dndice)

Apesar de serem postos como sinônimos, o JavaScript e o ECMAScript não possuem tal relação pois como podemos observar na ilustração abaixo, o JavaScript é a junção do ECMAScript (no caso o núcleo), o DOM (Document Objetc Model) e o BOM (Browser Object Model).

![js-ecma-dom-bom](http://i.imgur.com/78YVXKG.png)

### ECMAScript [◮](#%C3%8Dndice)

É uma linguagem de script que não é ligada somente aos navegadores. Ela forma a base do JavaScript, e foi padronizada pela organização [Ecma International](http://www.ecma-international.org/) na especificação **ECMA- e ECMA-402.**

Cuida basicamente das seguintes partes da linguagem:

* Sintaxe
* Tipos
* Statements (afirmações)
* Palavras-chave
* Palavras reservadas
* Operadores
* Objetos
