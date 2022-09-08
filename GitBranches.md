# Crear Ramas y movernos entre ellas en Git

Para crear una rama es tan simple como:

```
git branch branch_name
```

Y para moverme a esa rama basta con:

```
git checkout branch_name
```

Un comando muy util para crear una rama y ala vez moverme a la misma es 

```
git ckeckout -b branch_name
```

### Hacer merge nuestras ramas


Para hacer un merge entre ramas, lo primero es definir a que rama quiero hacer el merge
digamos si estoy en develop y quiero conectarme a master entonces me tendre que cambiar a 
master y luego hacer el siguiente comando:

```
git merge develop -m "commit_message"
```

recordando que al hacer merge es como si hicieramos un commit, asi que debemos agregar un mensaje.

## Github y las ramas

### Subir ramas a Github

Para subir las ramas en GitHub unicamente debemos hacer un push de la rama:

```
git push origin branch_name
```
