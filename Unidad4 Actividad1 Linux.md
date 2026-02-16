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
