 **Estado do componente**

 *1 conceito*

 renderizar
 E quando o compenente e carregado em tela

 *2 conceito*

 Caso voce precise inserir 2 componentes filhos em 1 funcao ou componente
 voce precisa uma um fragment

```js
<>
<componente1>
<componente2>
</>
```
ele funciona como uma div so pro codigo, fica invisivel no codigo final

*3 conceito*

Atualizacao do codigo
O React nao fica verificando variaveis.
Ele n recarrega a pagina se nao for usado parametros especiais para isso

*Hooks*

No react existem os famosos hooks que sao os uses
O primeiro que vamos abordar e o useState pra atualizacao de variaveis

*boas praticas*

A comunidade decidiu que depois de destruturar uma variavel com os hooks 
a segunda variavel da array tem o nome comecando com set e depois o mesmo nome da 
primeira variavel mas com letra maiuscula
exemplo:
```js
const [counter, setCounter] = useState(0);
```
No caso do useState o primeiro valor e uma variavel e o segundo uma funcao pra atualizar a variavel

Um Jeito de facilitar a atualizacao da variavel e simplificar usando
o valor anterior(proprio do useState, ele salva o valor anterior e o valor atualizado)

```js
function increment(){
  setCounter((valorAnterior)=>valorAnterior+1);
}
```
ao inves de

```js
fucntion increment(){
    setCounter(counter + 1);
}
```