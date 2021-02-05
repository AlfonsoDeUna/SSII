# Clase fecha: 05_02

### listar ficheros

```
Get-ChildItem -Force c:\
Get-ChildItem -Force c:\ -Recurse
```

### Buscar ficheros a partir de una determinado filtro 

* A partir de una fecha
```
Get-ChildItem -Force c:\ | Where-Object -FilterScript {($_.LastWriteTime -gt '2005-10-01')}
```

* longitud mayor a un 1 mega

```
 ($_.Length -ge 1mb)
 
 ($_.Length -le 100mb)
 ```
 


### Crear ficheros

```
  New-Item -Path 'C:\temp\New Folder' -ItemType Directory
  New-Item -Path 'C:\temp\New Folder\file.txt' -ItemType File
```

Obtener todos los ficheros
---

Get-ChildItem -Path $env:ProgramFiles -Recurse -Include *.exe | Where-Object -FilterScript {($_.LastWriteTime -gt '2005-10-01') -and ($_.Length -ge 1mb) -and ($_.Length -le 10mb)}

## PARTICIONES DE DISCO DURO

### GPT 
https://www.profesionalreview.com/2019/01/16/particion-gpt/

Get-Disk

* 1. Inicializar y darle una partición

```
Initialize-Disk -Number 1 -PartitionStyle GPT
```

* 2. Crear partición

```
New-Partition -DiskNumber 1 -Size 50GB -AssignDriveLetter
```

* 3. Formatear la partición

``` 
Format-volume -DriveLetter E -FileSystem NTFS
``` 



