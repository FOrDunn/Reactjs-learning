**imutabilidade no React**

A imutabilidade diz que uma variavel nunca vai poder ter seu valor alterado,
mas sim receber um novo valor

exemplo:

```js
usuarios = ['nome', 'nome2', 'nome3']

usuarios.push('nome4')

novoUsuarios = [...usuarios, 'nome4']
```
