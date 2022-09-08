# Crear un repositorio en GitHub para tener un control de versiones en la nube

Para empezar crearemos un repositorio en github y copiaremos el link **HTTPS** en el caso
de este repositorio es:

[Repositorio Link](https://github.com/ChuzOP/Git-tests.git)

Luego verificar si tenemos alguna rama de tipo master y cambiarla a main, por y para fines prácticos con:

```
    git branch -M main
```

Y para bindear un repositorio en **GitHub** lo haremos con el comando:
```
    git remote add origin repository_link
```

Podemos confirmar el bindeo anterior con:
```
    git remote -v
```

Ahora para *pushear* nuestros archivos de nuestro repositorio local a nuestro repositorio en la nube:
```
    git push origin branch_name 
```
<!-- Tenemos que asignarle el nombre de la rama que queremos pushear -->

Tambien habran ocasiones en las que nos equivoquemos bindeando nuestros repositorios asi que para desbindear:
```
    git remote remove origin
``` 

### Jalar archivos desde el repositorio en la nube a mi repositorio local

Para hacer esto usaremos el **pull** a la rama donde queramos traer los elementos :
``` 
    git pull origin branch_name
```