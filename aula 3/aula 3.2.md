**Utilizando mais um hook(useEffect)**

*useState*

Uma listagem do useState sempre comeca com uma array vazia ou um vetor vazio

Sempre comecar com o mesmo tipo de dado que vai ser no final

exemplo:

boleano = boleano no usestate tbm

array = array dentro do state

etc

*useEffect*

Serve para disparar uma funcao quando algo acontecer

Use effect pode ser encaixada em qualquer lugar( em qualquer lugar do componente)

Ela recebe 2 parametros

-1 a funcao que vai executar

-2 quando ela vai executar

exemplo:
```js
useEffect(()=> {
    console.log("abc");
}, [repository]);
```
O primeiro parametro e a funcao, que neste caso e uma arrow function
o segundo parametro colocado fora da funcao e quando ela vai mudar, que neste caso
e a array de repositorios

Se o useEffect tiver o segundo parametro vazio(dentro da array) ele vai ser executado apenas 1 vez,
no momento em que o componente for exebido em tela
exemplo:
```js
useEffect(()=> {
    console.log("abc");
}, []);
```
Se o useEffect n tiver segundo parametro vai entrar em loop e executar infinitamente

exemplo:
```js
useEffect(()=> {
    console.log("abc");
});
```