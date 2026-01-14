# UNIDAD 3. ACTIVIDAD 1. EJERCICIOS CON DIRECTORIOS

## 1.- Crea un directorio llamado iso en tu unidad c:\. Sitúate en el directorio iso de tu unidad (que será la unidad C). Desde el directorio iso crea los directorios (1_eval, teoria, t1, practica, p1a, p1b)

```
 C:\>cd iso
````
## Situados en C:\iso creamos 1_eva

```
>md c:\iso\1_eval
```
##  Situados en C:\iso creamos teoria

```
md c:\iso\1_eval\teoria
```
## Situados en  C:\iso creamos t1

```
md c:\iso\1_eval\teoria\t1
```
## Situados en iso creamos practica, p1a, p1b

```
md c:\iso\1_eval\practica\p1a\p1b
```

## Nos situamos en p1b

```
>cd 1_eval\practica\p1a\p1b
```

## Creamos los directorios 3_eval, teoriaa, teoriab utilizando trayectorias relativas.

```
md ..\..\..\..\3_eval\teoriaa ..\..\..\..\3_eval\teoriab
```

## Crea y sitúate en el directorio 2_eval. Crea los directorios (prac1, prac2, prac3) con una única sentencia.

```
c:\iso>md 2_eval

c:\iso>cd 2_eval

c:\iso\2_eval>
```

## Crea los directorios (prac1, prac2, prac3) con una única sentencia.

```
md prac1 prac2 prac3
```
## 5.- Sitúate en el directorio prac3. Crea los directorios (prac31, prac311) usando trayectorias relativas.

```
Nos situamos en prac3

c:\>cd iso\2_eval\prac3

c:\iso\2_eval\prac3>
```
<img width="464" height="241" alt="imagen" src="https://github.com/user-attachments/assets/82bbd18b-2f2c-4998-8926-f4366157d0d9" />

## Creamos prac31 y prac311 usando trayectoria relativa:

``
c:\iso\2_eval\prac3>md prac31\prac311

```
## 6.- Accede al directorio iso usando trayectoria absoluta con una única sentencia.

```
c:\iso\2_eval\prac3>cd c:\iso

c:\iso>

```
<img width="413" height="268" alt="imagen" src="https://github.com/user-attachments/assets/5fff7937-24b7-4d27-a28a-968fa412c6fe" />

## 7.- Desde iso elimina los directorios (prac311, prac31, teoriab, teoriaa, t1, p1b, p1a) utilizando trayectorias absolutas.

Vemos el árbol de directorios
Eliminamos p1a utilizando trayectorias absolutas, al eliminar p1a, se borra también p1b

```
c:\iso>rd /s c:\iso\1_eval\practica\p1a

```
<img width="458" height="171" alt="imagen" src="https://github.com/user-attachments/assets/8cf66de5-30ae-4d7c-a4c2-e00d9619262e" />

## 8.- Accede al directorio 2_eval usando trayectoria relativa con una única sentencia.

```
c:\iso>cd 2_eval

c:\iso\2_eval>

```
## 9.- Desde aquí cambia el nombre del directorio prac1 por el de prac4.

```
c:\iso\2_eval>rename prac1 prac4

```
## 10.- Desde aquí sitúa el directorio prac4 dentro del directorio prac3.

```
move prac2 prac

```
## 11.- Desde aquí elimina los directorios (1_eval, 3_eval)

```
c:\iso\2_eval>rd /s /q c:\iso\1_eval ..\3_eval

```

## 12.- Ejecuta la orden para visualizar el árbol de directorios y subdirectorios dependientes del directorio iso

```
c:\iso\2_eval>tree c:\iso

```

## 13.- Accede directamente a la raíz (a la unidad en la que te encuentras)

```
c:\iso\2_eval>cd\

c:\> 

```
