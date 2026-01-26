# UNIDAD 3. ACTIVIDAD 5. EJERCICIOS CON DIRECTORIOS. POWERSHELL
## Nombre: Pablo Jiménez Martínez

## Actividad 1. Crea el siguiente árbol de directorios siguiendo las instrucciones paso a paso. En cada uno de los pasos deberás transcribir todas y cada una de las sentencias utilizadas.

```
New-Item -itemtype Directory c:\iso

```

```
Set-Location iso
```
```
 New-Item -itemtype Directory c:\iso\1_eval\teoria\t1, c:\iso\1_eval\practica\p1a\p1b
```
<img width="789" height="505" alt="imagen" src="https://github.com/user-attachments/assets/670399f7-6785-4312-ae3f-5604326af589" />

## 2.- Sitúate en el directorio p1b. Crea los directorios (3_eval, teoriaa, teoriab) utilizando trayectorias relativas.

```
 Set-Location c:\iso\1_eval\practica\p1a\p1b
```
```
New-Item -itemtype Directory ..\..\..\..\3_eval\teoriaa, ..\..\..\..\3_eval\teoriab
```

<img width="789" height="189" alt="imagen" src="https://github.com/user-attachments/assets/47e525c2-a468-4231-8983-e291df3ade77" />

## 3.- Sitúate en el directorio iso. Crea el directorio (2_eval).

```
PS C:\iso\1_eval\practica\p1a\p1b> Set-Location c:\iso

PS C:\iso> New-Item -itemtype Directory 2_eval
```

## 4.- Sitúate en el directorio 2_eval. Crea los directorios (prac1, prac2, prac3) con una única sentencia.

```

PS C:\iso> Set-Location 2_eval

PS C:\iso\2_eval> new-item -itemtype Directory prac1, prac2, prac3
```

## 5.- Sitúate en el directorio prac3. Crea los directorios (prac31, prac311) usando trayectorias relativas.

```
PS C:\iso\2_eval> Set-Location prac3

PS C:\iso\2_eval\prac3> new-item -itemtype Directory prac31, prac31\prac311
```

## 6.- Accede al directorio iso usando trayectoria absoluta con una única sentencia.

```
Set-Location c:\iso
```

<img width="326" height="34" alt="imagen" src="https://github.com/user-attachments/assets/95b240bd-2659-4ea3-8ae2-08766c1a901c" />

## 7.- Desde iso elimina los directorios (prac311, prac31,teoriab, teoriaa, t1, p1b, p1a) utilizando trayectorias absolutas.

```
 Remove-Item c:\iso\2_eval\prac3\prac31\prac311, c:\iso\2_eval\prac3\prac31, c:\iso\3_eval\teoriaa, c:\iso\3_eval\teoriab, c:\iso\1_eval\teoria\t1, c:\iso\1_eval\practica\p1a\p1b, c:\iso\1_eval\practica\p1a
```
## 8.- Accede al directorio 2_eval usando trayectoria relativa con una única sentencia.

```
Set-Location 2_eval
```
## 9.- Desde aquí cambia el nombre del directorio prac1 por el de prac4.

```
Move-Item prac prac5
```
<img width="419" height="190" alt="imagen" src="https://github.com/user-attachments/assets/4cec013f-f4a6-43be-ba77-46daae028139" />
Ya tenia prac4 por eso e puesto prac5

## 10.- Desde aquí sitúa el directorio prac4 dentro del directorio prac3.

```
Move-Item prac4 prac3
```
<img width="419" height="121" alt="imagen" src="https://github.com/user-attachments/assets/26da9a81-b95b-4691-aa9d-d7b24d07144d" />

## 11.- Desde aquí elimina los directorios (1_eval, 3_eval)

```
PS C:\iso\2_eval> Remove-Item -recurse c:\iso\1_eval, c:\iso\3_eval
```
<img width="476" height="116" alt="imagen" src="https://github.com/user-attachments/assets/9deb43d7-e9b4-4f7c-ae2b-da9d99daa80e" />

## 12.- Ejecuta la orden para visualizar el árbol de directorios y subdirectorios dependientes del directorio iso

```
tree C:\iso
```

Listado de rutas de carpetas

El número de serie del volumen es 00000086 9297:7166

C:\ISO

└───2_eval

├───prac2

└───prac3

└───prac4 
<img width="476" height="130" alt="imagen" src="https://github.com/user-attachments/assets/7e3c4257-7703-46e5-87be-9c91e77b0621" />

## 13.- Accede directamente a la raíz (a la unidad en la que te encuentras)

PS C:\iso\2_eval> Set-Location \

PS C:\>
<img width="476" height="43" alt="imagen" src="https://github.com/user-attachments/assets/f0eb1cf2-c9dc-40c4-b9c2-98b0d4d15651" />
