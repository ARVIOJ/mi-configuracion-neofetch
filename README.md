# Mi Configuración Neofetch

Bienvenido al repositorio de mi configuración personalizada de Neofetch en PowerShell. Aquí encontrarás todos los detalles para replicar esta configuración en tu sistema.

![Imagen preview de mi configuración de Neofetch en PowerShell](https://github.com/ARVIOJ/mi-configuracion-neofetch/blob/main/preview.png)

## 🚀 Instalación

Para comenzar, sigue estos pasos para instalar las herramientas necesarias y configurar tu entorno.

### Paso 1: Instalar Scoop, Git y Neofetch

Abre PowerShell y ejecuta los siguientes comandos:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression

scoop install git
scoop install neofetch
```

### Paso 2: Instalar Oh My Posh y la Fuente
Para instalar Oh My Posh y configurar la fuente, utiliza el siguiente comando:

```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```

Después, agrega oh my posh a las variables de entorno en Path:

```powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\jandedobbeleer.omp.json" | Invoke-Expression
```
Para instalar la fuente con el comando:

```powershell
oh-my-posh font install
```

Y seleccionar la fuente de preferencia.

### Paso 3: Configuración del Terminal

En la terminal de PowerShell presionar **'Ctrl + Shift + ,'** para abrir el archivo 'settings.json'. En el apartado **'schemes'** del archivo, buscar pinkTerminal y copiar todo lo que esté dentro de las llaves **{}**. Luego, pegar en el archivo que se abrió al presionar **'Ctrl + Shift + ,'** .

Después buscar el apartado font y colocar el nombre de la fuente, en mi caso es **'MesloLGM Nerd Font'**.

### Paso 4: Configurar Neofetch

Busca la carpeta de Neofetch, esta estará en:
Disco Local C://, Usuario, nombreUsuario, neofetch

Copia los archivos dentro de la carpeta Neofetch de este repositorio, tanto **'config.con'** como **'mandalorian-symbol-ascii-art'**. Pegarlos dentro de la carpeta Neofetch de su máquina pidiendo sobrescribir y aceptar.

### Paso 5: Configurar PowerShell Profile

Ejecutar el comando:

```powershell
New-Item -Path $PROFILE -Type File -Force

notepad $PROFILE
```

Pegar lo del archivo **'Microsoft.PowerShell_profile.ps1'**. Para guardar los cambios ejecutar el comando:

```powershell
notepad $PROFILE
```

```powershell
. $PROFILE
```

## 🌟 ¡Listo!
Con estos pasos, tendrás una terminal personalizada y lista para mostrar tu configuración Neofetch cada vez que inicies PowerShell.
