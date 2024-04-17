# Mi Configuración Neofetch

Bienvenido al repositorio de mi configuración personalizada de Neofetch en PowerShell. Aquí encontrarás todos los detalles para replicar esta configuración en tu sistema.

![Imagen preview de mi configuración de Neofetch en PowerShell](https://github.com/ARVIOJ/mi-configuracion-neofetch/blob/main/preview.png)

## 🚀 Instalación

Para comenzar, sigue estos pasos para instalar las herramientas necesarias y configurar tu entorno.

### Paso 1: Instalar Git y Neofetch

Abre PowerShell y ejecuta los siguientes comandos:

```powershell
scoop install git
scoop install neofetch

# instalar ohmyposh y fuente con el comando en la terminal de powershell:
winget install JanDeDobbeleer.OhMyPosh -s winget

despues agregar la variables de entorno en Path:
C:\Users\user\AppData\Local\Programs\oh-my-posh\bin

para instalar la fuente con el comando:
oh-my-posh font install

y selecionar la de preferencia

en la terminal de powershell presionar
ctrl + shift + ,
en el apartado schemes del archivo "settings.json" buscar "pinkTerminal" y copiar todo lo dentro de las llaves {} 
y copiar en el archivo que se abrio al presionar ctrl + shift + ,

depues buscar el aparatdo "font" y colocar el nombre de la fuente en mi caso es "MesloLGM Nerd Font"

depues buscar la carpeta neofetch esta estara en disco local C://, Usuario, nombreUsuario y neofetch

copiar los archivo dentro de la carpeta neofetch de este repositorio tanto config.conf como mandalorian-symbol-ascii-art

pegarlos dentro de la carpeta neofetch de su maquina pedira sobreescribir y aceptaran

por ultimo colar el comando:

notepad $PROFILE

pegar lo del archivo "Microsoft.PowerShell_profile.ps1"
y por ultimo para guardar los cambios  el coamando:

. $PROFILE
