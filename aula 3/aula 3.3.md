**Listagem de repositorios com api do github**

Precisamos percorrer a array de repositorios
Com o foreach vamos conseguir fazer isso mas n conseguiremos retornar nada e dar o display 
por isso precisamos do map


quando o retorno tem apenas uma linha so n precisamos colocar parenteses nem chaves,
podemos inserir o codigo direto na mesma linha

```js
{repositories.map(repository => <RepositoryItem repository={repository} />)}
```

ao inves de

```js
{repositories.map(repository => {
    <RepositoryItem repository={repository} />
})}
```

Ja dentro do nosso outro arquivo onde esa o componente dos itens
Podemos puxar os dados do repositorio com o proprio props

```js
export function RepositoryItem(props) {
    return(
        <li>
            <strong>{props.repository.name}</strong>
            <p>{props.repository.description}</p>

            <a href={props.repository.html_url}>
            Acessar repositorio
            </a>
        </li>
    );
}
```

Como cada item precisa ser diferenciado para o sistema conseguir memorizar melhor
precisamos passar uma key para eles

```js
{repositories.map(repository => {
    <RepositoryItem key={repository.name} repository={repository} />
});}
```