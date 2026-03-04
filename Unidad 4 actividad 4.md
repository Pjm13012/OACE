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
<img width="1024" height="99" alt="image" src="https://github.com/user-attachments/assets/d6d7e86e-3ab5-45ef-b2a5-1d5f69c8ce48" />

## 5- Cambia la carpeta de referencia de usuario, en mi caso de /home/alex a home/alex2

<img width="1024" height="163" alt="image" src="https://github.com/user-attachments/assets/3752e490-501e-4087-8d39-83c413bf8fbb" />

## 6- Intenta crear la carpeta “prueba” en /home/usuario2, en mi caso /home/alex2

<img width="1024" height="62" alt="image" src="https://github.com/user-attachments/assets/f51a4fe8-3d8f-4d6c-83be-68e2272b16be" />

## 7- Logueate con tu usuario y contraseña en mi caso (comando su)

<img width="970" height="79" alt="image" src="https://github.com/user-attachments/assets/a59e5490-94d5-4b64-ae36-1dabc43d6a37" />

## 8- Intenta crear ahora carpeta usuario

<img width="722" height="60" alt="image" src="https://github.com/user-attachments/assets/19f8af26-b355-4d52-839d-64d761b6031e" />


## 9- Volvemos a loguearnos como “administrador”

<img width="722" height="60" alt="image" src="https://github.com/user-attachments/assets/974da4ad-3f2d-4f4d-bd0e-303764ca1b55" />

## 10- Elimina tu usuario creado

<img width="722" height="78" alt="image" src="https://github.com/user-attachments/assets/5904fbf2-ca71-4e57-9764-3bc425f55796" />

