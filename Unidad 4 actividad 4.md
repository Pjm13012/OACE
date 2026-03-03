# Unidad 4 Activad 4 Gestión de Usuarios

## Nombre: Pablo Jiménez Martínez
## Curso 2ºFPB

## 1.- Crea en tu SO a un usuario con tu nombre (en mi caso alex). Contraseña 2fpb1234


Si nos fijamos se ha creado

· un usuario “pablo”

· un grupo “pablo”

· Se ha metido el usuario “pablo” en el grupo “pablo”

· Se he creado la carpeta de usuario alex en /home/alex

Podemos ver los diferentes usuarios del sistema en el archivo /etc/passwd

Con el comando cat /etc/passwd podemos revisar que el usuario alex se ha creado

<img width="925" height="500" alt="image" src="https://github.com/user-attachments/assets/a268ae3d-e974-4284-9dd8-9436ce8d52c6" />


Con el comando cat etc/group podemos ver que el grupo “pablo” se ha creado


Podemos ver que hay una carpeta llamada “pablo” en la carpeta de “home” del sistema.

Con el comando “id alex” vemos los grupos a los que pertenece el usuario “pablo”

En este caso, solo pertenece al grupo “pablo”

## 2- Crea el grupo grupotest


Creamos el grupo “grupotest” observamoos que el Group ID(GID) es el 1012
```
Si ejecutamos cat /etc/group vemos que se ha creado el grupo “grupotest”
```
<img width="298" height="302" alt="image" src="https://github.com/user-attachments/assets/145d514c-1c76-418a-9861-d789da1b135a" />

## 3- Metemos a tu usuario en el grupo “grupotest”


Observamos que pablo ya está en los grupos “alex” y “grupotest”

## 4- Cambia el nombre de tu usuario, por usuario2, en mi caso alex2


Comprobamos que alex ya no existe y se ha cambiado por alex2, también vemos que la carpeta de referencia sigue siendo alex
```
administrador@ServerAula3:~$ cat /etc/passwd
```
