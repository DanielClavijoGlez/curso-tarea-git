# Respuestas
### Cada número se corresponde a los pasos con una pregunta asociada.

11. git reset HEAD~1 && git restore git-nuestro.md, porque con el primero cambiamos a un commit exactamente un paso anterior y el otro comando deja el working copy como está en el commit actual, que es distinto al commit siguiente que es del que venimos.

12. git reflog && git reset “clave” && git restore git-nuestro.md. Primero hay que buscar el código del commit al que queremos ir, luego es la misma lógica que el paso 11, nos movemos a otro commit y dejamos el working copy tal como está el commit

13. porque primero se hicieron unos commits sobre main, luego se creó una nueva rama, que es donde se modifica el archivo, sin hacer nada en la rama main y luego se hizo el merge, lo que junta los cambios; si aquí se encuentra con que en main también se modificó el archivo, sí habría conflicto.

19 sí, porque a partir del primer commit del archivo en la rama main, este se modificó en las dos ramas que estamos juntando, por lo que no sabe con cual de los dos quedarse. No habría conflicto si , por ejemplo, la rama htmlify se hubiera creado desde styled y no desde main

21. no, porque aunque el archivo sea distinto en ambas ramas, los cambios en la rama styled se hicieron a partir de la última modificación en la rama main, sin hacer modificaciones en esta última.

25. git log –graph

26. Sí, porque solo hay que mover la rama main hacia el commit de la rama title para tener acceso a todos los anteriores, de hecho, en esencia el merge que se hizo es fast-forward

27. git reset HEAD~1

28. git restore git-nuestro.md

29. git branch -D title

30. git reflog && git reset “clave” && git restore git-nuestro.md

32. Buscamos la clave del commit en git log y vamos con git checkout

33. Lo mismo que el anterior pero buscamos la clave con git reflog