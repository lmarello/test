# TEST 1...

Un "commit" con "breaking changes" se refiere a aquellos cambios que incluyen modificaciones que pueden afectar la compatibilidad con versiones anteriores o el funcionamiento del código existente.

Ante estos casos es importante agregar una descripción al commit de cual es el `breaking change`.
Para ello podemos realizarlo de la siguiente manera.

```console
git commit -m "feat: add some feature" -m "BREAKING CHANGES: The 'dummyFn' function returns an error 500 instead of 400"
```

- El segundo argumento `-m` se asigna a la descripción de dicho `commit`.

En los casos en que mergeemos un `pull-request` que posee un `breaking change`, asegurarse de que el mensaje del `squash/rebase commit` tenga el mensaje en la primera línea.

Ejemplo:

"BREAKING CHANGE" en la descripción
