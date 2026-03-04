# Unidad 4 Actividad 2 Linux
## Nombre: Pablo Jiménez Martínez
## Curso: 2ºFPB

## 1.- Situado en smm crea los directorios A, B, C, D, A1, A2, A3, B1, B11, B111, B112, A21, A22, A221 con trayectorias relativas.

```
mkdir -p A/A1 A/A2/A21 A/A2/A22/A221 A/A3 B/B1/B11/B111 B/B1/B11/B112 C D
```
<img width="826" height="344" alt="image" src="https://github.com/user-attachments/assets/9832f410-fef5-4c23-a2b9-7a4e88e2cd5b" />

## 2.- Situado en A1 crea en A21 un fichero llamado o1 que contenga “Fernando” en la primera línea, “Zoraida” en la segunda línea y “Antonia” en la tercera línea. UTILIZA LAS REDIRECCIONES. Almacena el fichero o1 ordenado

```
Paso 1: echo -e "Fernandoq\nZoraida\nAntonia"

Paso 2: no está ordenado, vamos a ordenarlo:

echo -e "Fernando\nZoraida\nAntonia" | sort
```
Finalmente redireccionamos a un archivo y en otra orden se mueve o1 a C/Orden
```
echo -e "Fernando\nZoraida\nAntonia" | sort > A21/o1
```
<img width="890" height="140" alt="image" src="https://github.com/user-attachments/assets/09a79ebb-b301-4dd6-b29e-1b6aa791881b" />


## 3.- Crea una copia de A dentro de D con el nombre nuevoA. A continuación elimina A.
```
cp -r A D
```
<img width="729" height="46" alt="image" src="https://github.com/user-attachments/assets/7e73e0b9-c52a-4a43-8dc0-1a85664e60bc" />

## 4.- ¿Cuántas líneas contiene el fichero o1?¿Cuantas palabras?¿Cuantos caracteres?

<img width="890" height="235" alt="image" src="https://github.com/user-attachments/assets/0548be85-f3ff-474c-8815-c5a57bfb4910" />

## 5.- Crea en D un fichero llamado Nombre que contenga tu nombre y otro fichero llamado Apellido que contenga tu primer apellido.

<img width="890" height="333" alt="image" src="https://github.com/user-attachments/assets/06bf6dc5-7d88-4935-ae98-8cb8c51d041e" />

## 6.- Pon todos los permisos al propietario del fichero Nombre (mantén los permisos que tenían grupo y otros). Utiliza sistema octal.


## 7.- Pon sólo permiso de lectura (al propietario, grupo y otros) al fichero Apellido sin utilizar sistema octal.


## 8.- Elimina A1, A2 y A3 con trayectoria relativa y utilizando comodines.


## 9.- Mueve nuevoA dentro de C. Una vez movido cámbiale el nombre por A. Cambia el nombre de Apellido por el de apellido.

<img width="1024" height="503" alt="image" src="https://github.com/user-attachments/assets/3d72b2db-f994-4fae-8ea0-c0a51a010d4a" />

## 10.- Crea dentro de A los siguientes directorios “pasta”,”pasto”,”casta”, “casto”, “pasmo”, “casmo”


## 11.- Elimina todos los ficheros que existan

## 12.- Elimina todo lo que dependa de smm y con una única sentencia

## 13.- Crea un fichero vacío llamado vacio.txt (touch)

## 14.- Busca en el fichero Nombre cuantas “r” hay dentro del fichero. (revisa el comando grep -c)

<img width="1024" height="28" alt="image" src="https://github.com/user-attachments/assets/b4589563-4d07-413b-97c4-596f5e121182" />
