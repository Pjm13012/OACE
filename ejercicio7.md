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

## 🔹 Paso 3: Crear una contraseña segura

## Crea una contraseña de forma segura (no visible en texto plano):
```
$Password = Read-Host "Introduce la contraseña" -AsSecureString
```
## 🔹 Paso 4: Crear el usuario local

## Ejemplo: crear el usuario usuario_ps

```
New-LocalUser
```
 
 -Name: "usuario_ps" 
 -FullName: "Usuario de PowerShell" 
 -Description: "Cuenta creada desde PowerShell" 
 -Password: $Password
