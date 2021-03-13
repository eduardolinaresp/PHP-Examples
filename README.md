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