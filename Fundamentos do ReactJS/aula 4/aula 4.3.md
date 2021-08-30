**Tipagem em componentes**

Apesar de type ser muito usado, o mais comum no mercado hoje em dia ainda e o

```ts
interface RepositoryItemProps {
    repository: {
        name: string;
        description: string;
        html_url: string;
    }
}
```

O nome da interface e dado igual ao do componente e botado a props no final

Caso voce receba mais dados que deveria n e preciso adicionar a tipagem, voce so precisa fazer com os dados que vai utilizar este


Para adicionar um tipo ao estado(useState) precisamos passar com o generic(<NomeDaTipagemDaInterface>)

exemplo: 
```ts
useState<NomeDeUmaInterface>
```

e para deixar ele ser uma lista ou array precisamos botar o simbolo de colchetes no final
```ts
useState<NomeDeUmaInterface[]>
```
