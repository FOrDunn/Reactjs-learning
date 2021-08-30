**Fundamentos do Typescript**

typescript e um superset do javascript
Ou seja, o javascript com um pouco mais de funcoes e um tiquinho diferente

Para botar o tipo de algo voce usa

```ts
type
```

voce pode colocar o formato dos dados como se fosse um objeto
```ts
type User = {
    name: string
    email: string
    adress: {
        city: string
        state?: string
    }
}
```

Nesse ultimo (user.adress.state) botamos o sinal de que n e obrigatorio

E para aplicar ela em algum lugar voce usa os :

exemplo:

```ts
function showWelcomeMessage(user: User);
```

*Na maioria das vezes nao vamos usar o typescript em producao, so em desenvolvimento*


O typescript facilita muito a codar e deixa tudo bem mais fluido para ter menos erros

Ele tbm tem uma ferramente automatica de tipagem, ou seja, Ele faz tipagem automatica reconhecendo o valor da variavel