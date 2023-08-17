# Script_Pag_Sep
Repositorio para realizar la descarga de los libros de la página de la SEP de la clase Seguridad Informática.

Para el uso de este script se requiere tener instalada la última versión de Python.

Para las librerías se requiere tener BeautifulSoup y requests.

Iniciando actualizamos el Ubuntu con los comandos sudo apt update y sudo apt upgrade.

Estando dentro del servidor le instalamos las líbrerias que vamos a ocupar (BeautifulSoup y requests) con los siguientes comandos:
pip install requests
pip install beautifulsoup4

pasamos a realizar la instalación de Git con el comando:
sudo apt install git

Luego instalamos Python en el servidor con el comando siguiente,para que pueda ejecutar el script que teníamos de la clase anterior:
sudo apt install python

Revisamos la versión de git que fue instalada en el servidor con el comando :
python3 --version

Creamos una llave SSH para la coneccion con el servidor con el comando:
ssh-keygen -t rsa -b 4096 -C "Correo@usuario.com"

Buscamos la ubicación de la llave que acabamos de crear:
cat ~/.ssh/id_rsa.pub

Guardamos en la cuenta de github la llave que generamos.

Estando en github entramos al repositorio en donde esta el script de la clase y dando click en el botón Code obtenemos el SSH para poder clonar el repositorio en el servidor: 
git clone git@github.com:Bananas-En-Pijamas/Script_Pag_Sep.git

y procedemos a clonar el repositorio en el servidor

Ya con el repositorio clonado procedemos a buscar la carpeta y el Script.

Y ejecutamos el script "python3 Script.py"