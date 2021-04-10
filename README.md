
#Inicializar proyecto 

##- Inicializar contenedores

	docker-compose up 
	
##- comprobar  estado contenedor

    docker ps -a -f name=mysql_test

##- Acceder a contenedor

    docker exec -i -t mysql_test bash
	docker exec -i -t phpsoap_apache_1 bash
	

##- Detener de forma masiva

    docker ps -a -q | ForEach { docker stop $_ }
	
##- Conexion a BD por terminal

	mysql -u root -p	
	
## Comentarios
   En Este caso requerí instalar librerias adicionales entonces fui agregandolas 
   y recreando el contenedor con:
   
   docker-compose build apache
   
## Instalar composer 
   Documentacion
   https://linuxize.com/post/how-to-install-and-use-composer-on-debian-10/		
### Ejecutar
   apt-get install software-properties-common
   php composer-setup.php --install-dir=/usr/local/bin --filename=composer

## ADD phpspreadsheet SO

	

	


