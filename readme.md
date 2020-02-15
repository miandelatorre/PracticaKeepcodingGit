- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

He utilizado el comando 'git reset --hard HEAD~1'. Porque con reset le digo que vuelva atrás, con HEAD~1 le digo que vuelva como estaba antes de hacer el último commit y con '--hard' le digo que modifique mi working copy.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

He usado en primer lugar el comando 'git reflog', para ver un listado de todos los movimientos que se han realizado en el repositorio.
Posteriormente he usado el comando 'git reset --hard 1a47132', donde 1a47132 es el commit hash del último commit realizado. Para volver al último commit realizado.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
∑
No causó ningún conflicto. Porque desde que se creó la rama styled desde la rama master, la rama master todabía no se ha modificado.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Sí que se han generado conflictos. Porque los ficheros git-nuestro.md que se encuentran en los HEAD's de las ramas htmlify y styled son distintos.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

A mí me ha hecho un hecho un fast-forward, ha insertado nueve lineas y ha borrado nueve líneas, dejando el fichero de la rama master como la última vez que se subió a la rama style. Esto puede ser debido a que realmente el fichero que se encuentra en la rama style es realmente el mismo que se encontraba en la rama master, aunque con más carácteres, y lo que ha hecho ha sido añadir estos carácteres al fichero de la rama master.

- ¿Qué comando o comandos utilizaste en el paso 25?

El comando que utilizé es 'git log --graph'

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

Sí, podría haber sido fast forward, porque la rama master no fue modificada desde ningún commit que fue realizado en la rama title, y la rama title partió de la rama master.

- ¿Qué comando o comandos utilizaste en el paso 27?

git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28? 

git reset --hard HEAD

- ¿Qué comando o comandos utilizaste en el paso 29? 

git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30? 

Primero 'git reflog' para saber la referencia del nodo al que tengo que volver, que en mi caso es 68ac953, en este nodo se hizo el merge de la rama master con la rama title.
Luego he utilizado el comando 'git checkout 68ac953' para volver a ese nodo. 

- ¿Qué comando o comandos usaste en el paso 32?

Primero 'git reflog' para conocer la referencia de reflog que corresponde al commit inicial cuando se creó el poema, que en mi caso es f86919e.
Luego he utilizado el comando 'git checkout f86919e'

- ¿Qué comando o comandos usaste en el punto 33?
 Primero 'git reflog' para conocer la referencia de reflog que corresponde al estado final, cuando se puso título al poema, que en mi caso es ccce186.
Luego he utilizado el comando 'git checkout ccce186'

