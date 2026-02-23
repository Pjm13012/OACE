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
<img width="826" height="329" alt="image" src="https://github.com/user-attachments/assets/1175d32c-6fd4-46a8-a76c-031959dca671" />
No me deja redireccionarlo

## 3.- Crea una copia de A dentro de D con el nombre nuevoA. A continuación elimina A.
```
cp -r A D
```
<img width="729" height="46" alt="image" src="https://github.com/user-attachments/assets/7e73e0b9-c52a-4a43-8dc0-1a85664e60bc" />

## 
