# Git Stash
## Git stash es una forma de guardar los cambios que hayas hecho en una rama pero no quieres guardarlos en ese momento

Git stash nos es util cuando hacemos cambios pero no tenemos manera de deshacerlos y queremos voler a el ultimo commit que se
haya hecho

Hacer un stash unicamente se puede hacer, haciendo cambios en archivos ya creados con el comando:

```
git stash
```

Pero tambien podemos ponerle un mensaje al stash, para poder diferenciar entre varios o diferentes stash que tengamos, con el comando:

```
git stash save "message"
```

## Obtener elementos del Stash
<hr />

El stashed se comporta como una Stack de datos comportándose de manera tipo LIFO (del inglés Last In, First Out, «último en entrar, primero en salir»), así podemos acceder al método pop.

El método pop recuperará y sacará de la lista el último estado del stashed y lo insertará en el staging area, por lo que es importante saber en qué branch te encuentras para poder recuperarlo, ya que el stash será agnóstico a la rama o estado en el que te encuentres, siempre recuperará los cambios que hiciste en el lugar que lo llamas.
Entonces para traer el ultimo stash en la lista, lo hariamos con el comando:
```
gi stash pop
```

Tambien podemos ver los stash listados con el comando:
```
git stash list
```

Para sacar los cambios de un stash especifico usamos el comando:
```
git stash pop stash@{num_stash}
```
Donde *num_stash* es el indice que tiene el stash en la *stash list*

## Crear una rama con el o los stash
<hr/>

Para crear una rama y aplicar el stash mas reciente podemos utilizar el comando:
```
git stash branch_name
```

Tambien puedes crear una rama con un stash especifico con el comando:

```
git stash branch_name stash@{num_stash}
```

## Eliminar elementos del stash
<hr />

Para eliminar el ultimo elemento del stash con el comando:
```
git stash drop
```
Pero si solo quieres eliminar un stash lo puedes hacer con el indice del stash a eliminar:

```
git stash drop
```

Si quieres eliminar todos los elementos que haya en el stash, sería con el comando:
```
git stash clear
```