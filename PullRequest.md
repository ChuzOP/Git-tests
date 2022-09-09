# Pull Request
Es una funcionalidad de github (en gitlab llamada merge request y en bitbucket push request), en la que un colaborador pide que revisen sus cambios antes de hacer merge a una rama, normalmente master.

Al hacer un pull request se genera una conversación que pueden seguir los demás usuarios del repositorio, así como autorizar y rechazar los cambios.

## Datos importantes de los Pull Request
-Los PullRequest no generan un Merge, es un preludio a este para revisar los cambios.
-Dentro de los PullRequest se puede hacer un review para analizar los commits y cambios, esto permite entender qué es lo que se espera fusionar.
-Si un PullRequest no es aprobado, se deben realizar los cambios, hacer un pull y luego si un push para que se vuelvan a evaluar.
-Si un PullRequest es aprobado, pasa a la siguiente etapa de hacer merge.

## Flujo de Trabajo de un pull request:
1. Crear un Pull Request
2. Se hace una revisión de los cambios.
3. Se toma una decisión ( ya sea aceptar o rechazar los cambios)
    1. Si se rechazan los cambios se debe corregir los errores y volver al paso 2
    2. Si se aceptan los cambios, se procederá a hacer un merge 
