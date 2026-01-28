# UNIDAD 3. ACTIVIDAD 7. CREACIÓN USUARIOS POWERSHELL

## NOMBRE: Pablo Jiménez Martínez 2ºFPB

# ACTIVIDAD 1

## 📝 DESARROLLO DE LA ACTIVIDAD

## 🔹 Paso 1: Abrir PowerShell como administrador

1. Pulsa Inicio

2. Escribe PowerShell

3. Haz clic derecho → Ejecutar como administrador

## 🔹 Paso 2: Comprobar usuarios existentes

## Ejecuta el siguiente comando para listar los usuarios locales:
```
Get-LocalUser
```

Identifica que el usuario que vas a crear no exista previamente.

<img width="835" height="130" alt="image" src="https://github.com/user-attachments/assets/450d0107-3687-449a-8442-42bc6b868944" />

## 🔹 Paso 3: Crear una contraseña segura

## Crea una contraseña de forma segura (no visible en texto plano):
```
$Password = Read-Host "Introduce la contraseña" -AsSecureString
```
<img width="637" height="58" alt="image" src="https://github.com/user-attachments/assets/480fc7ce-1d87-4cac-a3bc-c899f742b89d" />

## 🔹 Paso 4: Crear el usuario local

## Ejemplo: crear el usuario usuario_ps

```
New-LocalUser
```
 
 -Name: "usuario_ps" 
 -FullName: "Usuario de PowerShell" 
 -Description: "Cuenta creada desde PowerShell" 
 -Password: $Password

## 🔹 Paso 5: Añadir el usuario a un grupo

## Para añadirlo al grupo Usuarios:

```
Add-LocalGroupMember -Group "Users" -Member "usuario_ps"
```

O al grupo Administradores ( solo si es necesario):

```
Add-LocalGroupMember -Group "Administrators" -Member "usuario_ps"
```
