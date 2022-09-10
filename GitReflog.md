# Git nunca olvida
Git guarda todos los cambios aunque decidas borrarlos, al borrar un cambio lo que estás haciendo sólo es actualizar la punta del branch, para gestionar éstas puntas existe un mecanismo llamado registros de referencia o **reflog**.

Para ver los registros cuándo se actualizaron las referencias de Git en el repositorio local (sólo en el local), por lo que si deseas ver cómo has modificado la historia puedes utilizar el comando:
```
git reflog
```

## Volver a una parte de la historia!!
<hr/>

Hay ocasiones en las que cometemos errores, y tambien habran veces que cometamos atrocidades y hacer commit de esas atrocidades, pero tranquilo 
la solución es hacer un reset, con el reset puedes volver a un punto en la historia de tu proyecto.

Hay 2 tipos de resets, el *hard* y el *soft*, el hard Perderá todo lo que se encuentra en staging y en el Working directory y el soft  recuperará todos los cambios que tengas diferentes al commit y los agregará al staging area.

```
git reset --hard ref_commit
git reset -soft ref_commit
```

Conclusión usa git reset, solo despues de que todo se fuera al carajo.