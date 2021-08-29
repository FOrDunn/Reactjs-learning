**Propriedades no React**

Sao informacoes variaveis para um componente funcionar de uma forma diferente

Para passar informacoes para um item filho voce deve passar um (props)
para ele conseguir levar os dados
```js
function componente(props) {
    return <h1>hello World</h1>
 }
```
Todos os dados inseridos no filho dentro do componente pai sao passados pelo props
Isso signfica que voce pode botar uma propriedade com o nome batata que ele vai passar e voce vai poder chamar

*exemplo de chamada pela propriedade*

props.batata
props.repositorio

*boas praticas*

quando se tem muitas propriedades e bom quebrar linha
Torna o codigo mais legivel e facil de ajustar

```js
<RepositoryItem
repository="uniform2"
description="Forms in React"
Link="https://github.com/">
```
