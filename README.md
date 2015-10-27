# chuleta-docker


`docker version` muestra la versión y detalles de docker

`docker --help` muestra ayuda
	`docker COMANDO --help` ...del comando de docker COMANDO


`docker images` Lista imágenes

`docker rmi IMAGEN` borra IMAGEN


`docker ps` Lista contenedores (sólo los activos)

	`docker ps -a` Lista contenedores (todos)

	`docker ps -l` Lista el último contenedor creado (activo o no)

`docker run IMAGEN COMANDO` Crea un contenedor a partir de IMAGEN, ejecuta COMANDO en él y muestra el resultado (y termina)

	`docker run -t -i IMAGEN COMANDO` ...de forma interactiva (`-i` mantiene STDIN abierto y `-t` asigna un terminal virtual en el contenedor)

	`docker run -d IMAGEN COMANDO` ...en modo daemon (sin mostrar el resultado)

	`docker run -P IMAGEN COMANDO` ...mapea los puertos necesarios (se muestran en un `ps`)

	`docker run -p 80:1080 IMAGEN COMANDO` ...mapea los puertos indicados



`docker stop CONTENEDOR` detiene CONTENEDOR

`docker start CONTENEDOR` inicia CONTENEDOR

`docker restart CONTENEDOR` reinicia CONTENEDOR

`docker rm COMTENEDOR` borra CONTENEDOR



`docker logs CONTENEDOR` Muestra un log con las salidas de CONTENEDOR

	`docker logs -t CONTENEDOR` ...con timestamp

`docker top CONTENEDOR` muestra los procesos en el contenedor
