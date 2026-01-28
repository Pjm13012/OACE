# Actividad 6 
## Nombre:Pablo Jiménez Martínez 2ºFPB 

## 1.- Situado en smm crea los directorios A, B, C y D. Utiliza trayectoria absoluta. 
```
c:\>cd smm

c:\>md c:\smm\a c:\smm\b c:\smm\c c:\smm\d

PS C:\> Set-Location c:\smm

PS C:\smm> New-Item -itemtype Directory c:\smm\a, c:\smm\b, c:\smm\c, c:\smm\d<img width="906" height="634" alt="imagen" src="https://github.com/user-attachments/assets/b0189232-8b22-4395-8009-5f25b333614a" />

```
<img width="678" height="319" alt="imagen" src="https://github.com/user-attachments/assets/244d5898-29fe-4a19-a75f-a85b979295cb" />

## 2.- Sitúate en D y desde allí crea A1, A2, A21, A22, A221 con una única sentencia utilizando trayectoria relativa.
```
c:\smm> cd d

c:\smm\d>md ..\a\a1 ..\a\a2\a21 ..\a\a2\a22\a221

PS C:\smm> Set-Location d

PS C:\smm\d> New-Item -itemtype Directory ..\a\a1, ..\a\a2\a21, ..\a\a2\a22\a221
```
<img width="678" height="370" alt="imagen" src="https://github.com/user-attachments/assets/327c7a5a-844d-4551-8983-76173b024a6a" />

## 3.- Sitúate en A221 y desde allí crea B1, B11, B111, B112 con una única sentencia y utilizando trayectoria relativa.
```
PS C:\smm\d> Set-Location c:\smm\a\a2\a22\a221

PS C:\smm\a\a2\a22\a221> New-Item -itemtype Directory ..\..\..\..\b\b1\b11\b111,

..\..\..\..\b\b1\b112
```

## 4.- Estando situado en A221, crea un fichero llamado lineas.txt en el directorio C que contenga el árbol de directorios dependiente del directorio A (incluyendo los subdirectorios).

```
PS C:\smm\a\a2\a22\a221> tree c:\smm\a > c:\smm\c\lineas.txt
```
<img width="444" height="34" alt="image" src="https://github.com/user-attachments/assets/667b0575-ff0b-466c-953a-1496ee16daef" />

## 5.- Crea en D un fichero llamado Nombre.txt que contenga tu nombre y otro fichero llamado Apellido.txt

```
PS C:\smm\a\a2\a22\a221> Set-Content c:\smm\d\nombre.txt "Alex"

PS C:\smm\a\a2\a22\a221> Set-Content c:\smm\d\apellido.txt "Lopez"
```
<img width="495" height="34" alt="image" src="https://github.com/user-attachments/assets/2bdca399-3e99-460c-996d-cd8eeac3d43a" />

## 6.- Genera un fichero llamado union.txt en D que contenga nombre y tu primer apellido.

```
PS C:\smm\a\a2\a22\a221> Get-Content c:\smm\d\nombre.txt > c:\smm\d\union.txt

PS C:\smm\a\a2\a22\a221> Get-Content c:\smm\d\apellido.txt >> c:\smm\d\union.txt
```
<img width="570" height="35" alt="image" src="https://github.com/user-attachments/assets/f99bf8c2-a7d8-472a-abaa-e8a0e52bde15" />
<img width="570" height="50" alt="image" src="https://github.com/user-attachments/assets/1fa3b81e-75b7-4e4f-963a-ce90a7f6319e" />

## 7.- Mueve el fichero union.txt a A21

```
PS C:\smm\a\a2\a22\a221> Move-Item c:\smm\d\union.txt c:\smm\a\a2\a21
```
<img width="560" height="28" alt="image" src="https://github.com/user-attachments/assets/ceadf8af-fd3c-4b1b-acc9-1b76666242c1" />

## 8.- Mueve el directorio A2 dentro de C.

```
Set-Location c:\smm

Move-Item c:\smm\a\a2 c:\smm\c
```

<img width="560" height="41" alt="image" src="https://github.com/user-attachments/assets/d7f18bcf-fd46-4736-ab4b-123f3922d65d" />

## 9.- Cambia el nombre del fichero union.txt por el de nuevaunion.txt

```
Rename-Item c:\smm\c\a2\a21\union.txt nuevaunion.txt
```
<img width="560" height="28" alt="image" src="https://github.com/user-attachments/assets/91cbb181-969b-4bc4-b838-104798523d1c" />

## 10.- Copia el fichero Nombre.txt al directorio A.

```
Copy-Item c:\smm\d\nombre.txt c:\smm\ a
```
<img width="560" height="28" alt="image" src="https://github.com/user-attachments/assets/04e4844a-4c8d-435e-aa6c-883ceb70491c" />
