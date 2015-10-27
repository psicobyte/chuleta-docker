# chuleta-docker

`docker images` Lista imágenes

`docker ps` Lista contenedores (sólo los activos)
	`docker ps -a` Lista contenedores (todos)
	`docker ps -l` Lista el último contenedor creado (activo o no)

`docker run IMAGEN COMANDO` Crea un contenedor a partir de IMAGEN, ejecuta COMANDO en él y muestra el resultado (y termina)
`docker run -t -i IMAGEN COMANDO` Crea un contenedor a partir de IMAGEN y ejecuta COMANDO en él de forma interactiva (`-i` redirige STDIN y `-t` asigna un terminal en el contenedor)
`docker run -d IMAGEN COMANDO` Crea un contenedor a partir de IMAGEN y ejecuta COMANDO en él en modo daemon (sin mostrar el resultado)
