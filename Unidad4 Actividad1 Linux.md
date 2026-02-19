# Unidad 4 Actividad 1 Linux
## Nombre: Pablo Jiménez Martínez
## Curso: 2ºFPB

## 1.- Crea el directorio SMM en tu directorio de usuario. Desde el directorio SMM crea los directorios (1_eval, teoria, t1, practica, p1a, p1b) utilizando trayectorias absolutas y una única sentencia.

```
mkdir SMM -> mkdir –p /home/user/SMM/1_eval/teoria/t1 /home/user/SMM/1_eval/practica/p1a/p1b
```
<img width="1113" height="150" alt="image" src="https://github.com/user-attachments/assets/91d6f1e6-3405-4719-b08c-b7a0cb485114" />

## 2.- Desde el directorio p1b crea los directorios (3_eval, teoriaa, teoriab) utilizando trayectorias relativas.

```
mkdir –p ../../../../../3_eval/teoriaa/teoriab/
```
<img width="922" height="20" alt="image" src="https://github.com/user-attachments/assets/77b525a3-43b2-4cfe-86db-853053902b28" />

## 3.- Desde el directorio SMM crea el directorio (2_eval).

```
mkdir 2_eval
```
<img width="476" height="238" alt="image" src="https://github.com/user-attachments/assets/281eead0-7f12-40c5-8766-382fa309ec6d" />

## 4.- Accede al directorio 2_eval. Desde aquí crea los directorios (prac1, prac2, prac3) con una única sentencia.

```
cd /home/user/SMM/2_eval

mkdir –p prac1 prac2 prac3
```
<img width="586" height="167" alt="image" src="https://github.com/user-attachments/assets/00f1c540-6713-4c52-8792-ed2f9c8e6155" />

## 5.- Accede al directorio prac3. Desde aquí crea los directorios (prac31, prac311) usando trayectorias relativas.

```
cd prac3

mkdir -p prac31/prac311
```
<img width="586" height="167" alt="image" src="https://github.com/user-attachments/assets/728f790c-7e7c-4790-9c34-2bd42de71974" />

## 6.- Accede al directorio SMM usando trayectoria absoluta con una única sentencia.

```
cd /home/user/SMM/
```
No me dejaba hacerlo
<img width="597" height="116" alt="image" src="https://github.com/user-attachments/assets/01b10942-5aa2-40e8-a9eb-eea6f2904b5a" />

## 7.- Desde aquí elimina los directorios (prac311, prac31, teoriab, teoriaa, t1, p1b, p1a) utilizando trayectorias absolutas.

```
rm -r /home/user/SMM/2_eval/prac3/prac31 /home/user/SMM/3_eval/teoriaa/ /home/user/SMM/1_eval/teoria/t1/ /home/user/SMM/1_eval/practica/p1a/
```
<img width="1009" height="377" alt="image" src="https://github.com/user-attachments/assets/254d67a9-7a8b-40a6-b76a-81693c621363" />

## 8.- Accede al directorio 2_eval usando trayectoria relativa con una única sentencia.

```
cd 2_eval/
```
<img width="1009" height="41" alt="image" src="https://github.com/user-attachments/assets/a9a336f5-f885-4d1d-91d6-9e205ca1e9a9" />

## 9.- Desde aquí cambia el nombre del directorio prac1 por el de prac4. (El comando sería el mv →investiga en la ayuda de Linux. Recuerda que el comando de ayuda es man).

```
mv prac1 prac4
```
<img width="461" height="48" alt="image" src="https://github.com/user-attachments/assets/affec895-207c-452e-a93e-b60d19ec219f" />

## 10.- Desde aquí sitúa el directorio prac4 dentro del directorio prac3.
```
mv prac4 prac3
```
<img width="442" height="50" alt="image" src="https://github.com/user-attachments/assets/f22a2f08-5d52-4042-9bc0-4a352c4166dd" />

## 11.- Desde aquí elimina los directorios (1_eval, 3_eval)
```
rm –r ../1eval ../3eval
```
<img width="722" height="258" alt="image" src="https://github.com/user-attachments/assets/36d70c01-b200-41a0-b103-fad65aa4a1e0" />

## 12.- Consulta la ayuda del comando cal (Recuerda que el comando de ayuda es man). Utiliza dicho comando para visualizar el calendario del mes de enero de 2021.
```
man cal
```
<img width="983" height="497" alt="image" src="https://github.com/user-attachments/assets/248455d3-c346-4625-80dd-b7ae8b4d4683" />

*SI pide instalar cal --> apt install ncal

## 13.- Ejecuta el comando cal y redirecciónalo a un fichero llamado calendario.

cal > calendario
