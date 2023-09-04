# AREP-Taller-3
En este taller se tuvo como objetivo realizar un servidor web que respondiera a las peticiones con archivos y servicios.

Este taller es una continuacion del primero [AREP Taller 2](https://github.com/JuanPabloDaza/AREP-Taller-2).

## Para ejecutar el programa

Se puede hacer uso del comando git clone y usar la URL del repositorio:
```
https://github.com/JuanPabloDaza/AREP-Taller-2
```

## Prerequisitos

Es necesario tener instalado maven para compilar y probar los test del programa, si no se tiene maven puede instalar [aqui](https://maven.apache.org/install.html).

## Instalacion 

Una vez clonado, se debe hacer uso del comando:

```
mvn package
```

Este comando compilara el programa y tambien ejecutara las pruebas. 

## Despliegue del programa:

Para ejecutar el programa se usa el comando:

```
mvn exec:java -D "exec.mainClass"="edu.escuelaing.arep.ASE.app.HttpServer"
```
Una vez ejecutado se debe acceder a traves de un buscador y con la direccion:
```
127.0.0.1:35000
```

## Descripcion del programa:

### Diseño:

En este programa se usa la clase HttpServer para responder las solicitudes POST que sean necesarias, dentro de la pagina principal hay un buscador que permite ingresar el valor en el servicio que se desea usar.

Se utilizan funciones lambda para crear los servicios. Dentro del metodo initilizeServices() de la clase HttpServer se especifican los servicios disponibles.

## Construido con:

* [Maven](https://maven.apache.org/) - Manejo de dependecias.
* [OMDb API](https://www.omdbapi.com/) - API Externa

## Autor

* Juan Pablo Daza Pinzon
