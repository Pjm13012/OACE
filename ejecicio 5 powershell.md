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
