# Actividad 6 
## Nombre:Pablo Jiménez Martínez 2ºFPB 

## 1.- Situado en smm crea los directorios A, B, C y D. Utiliza trayectoria absoluta. 
```
c:\>cd smm

c:\>md c:\smm\a c:\smm\b c:\smm\c c:\smm\d

PS C:\> Set-Location c:\smm

PS C:\smm> New-Item -itemtype Directory c:\smm\a, c:\smm\b, c:\smm\c, c:\smm\d
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
c:\smm\d>cd c:\smm\a\a2\a22\a221

c:\smm\a\a2\a22\a221> md ..\..\..\..\b\b1\b11\b111 ..\..\..\..\b\b1\b112

PS C:\smm\d> Set-Location c:\smm\a\a2\a22\a221
```

PS C:\smm\a\a2\a22\a221> New-Item -itemtype Directory ..\..\..\..\b\b1\b11\b111,

..\..\..\..\b\b1\b112
