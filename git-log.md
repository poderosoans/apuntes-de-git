### git log
Muestra todo el historial de commits del proyecto

`git log --pretty=format:"%h - %an, %ar : %s"`
Muestra el historial con el formato que indiquemos.


### Limitar la salida del historial
`git log -n`: Cambiamos la n por cualquier numero entero, por ejemplo `git log -2` nos mostrará los 2 commits más recientes.

`git log --after="2016-04-07 00:00:00"` Muestra los commits realizados después de la fecha especificada.

`git log --before="2016-04-07 00:00:00"` Muestra los commits realizados antes de la fecha especificada.

Las banderas del comando `git log` se pueden usar juntas según convenga, por ejemplo:

`git log --after="2017-07-10 11:00:00" --before="2017-07-11 22:30:00"`