# Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

## Zonas de Git

1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

## Flujo de trabajo básico en Git
1. Modificar los archivos
2. Preparamos los archivos
3. Confirmamos los cambios

## Configurando Git por primera vez

```
git config --global user.name "Roger Pomacarhua"
git config --global user.email roger.pomacarhua@gmail.com
git config --global core.editor nano
git config --list
```

## Configuración SSH en Windows
1. Creamos una carpeta llamda `llaves-ssh` en el disco `C` para evitar problemas de rutas.
2. Ejecutamos el comando `ssh-keygen -t rsa -C` "poderosoans@hotmail.com" (El correo debe ser el mismo con el que nos regirstramos en Github para evitar problemas.)
Dejamos el passphrase vacío y damos enter.
Cuando nos pida la ruta escribimos `/c/llaves-ssh/github_rsa`.
3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.
4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add /c/llaves-ssh/github_rsa`.
5. Desde ahora podemos hacer pull y push sin que Github nos esté piediendo los datos de acceso.