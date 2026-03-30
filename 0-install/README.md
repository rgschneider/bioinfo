# Archivos de instalación UNIX

Estos archivos se utilizan para que los alumnos puedan configurar sus computadoras e instalen los programas necesarios para la cursada de Bioinformática.

## Configuración de Bash

Hay dos versiones de los archivos de configuración de bash (`.bash-profile` y `.bashrc`) dependiendo de si va a ser utilizado en un entorno Linux (nativo o bajo Windows) o MacOS. Esos archivos están en dos carpetas diferentes:

	bash-files/linux/
	bash-files/macOS/
	
## Instalación de programas de bioinformática	
El archivo `conda.txt` coontiene un listado de los programas que se instalarán por medio de bioconda:

	xargs conda install -y
	
## Comprobación de la instalación

Se puede comprobar la correcta instalación y funcionamiento de los programas mediante el script `doctor.py` escrito por el Dr. István Albert.

Por recomendación este script se instala en la carpeta `~/bin` donde aconsejamos guardar todos los archivos binarios y scripts de uso general:

	mkdir -p ~/bin
	curl -L ...
	chmod +x ~/bin/doctor.py
	
Para usarlo sólo se deber correr:

	~/bin/doctor.py