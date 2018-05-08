# Course1718_e4a

| Modulo | Travis | Codacy | Codecov | Despliegue  |
|--|--|--|--|--|
| [Loader](https://github.com/Arquisoft/Loader_e4a)               | [![BuildStatus](https://travis-ci.org/Arquisoft/Loader_e4a.svg?branch=master)](https://travis-ci.org/Arquisoft/Loader_e4a)            | [![CodacyBadge](https://api.codacy.com/project/badge/Grade/f2f0d0b009384c8aba7deacb39b7b541)](https://www.codacy.com/app/Llambi/Loader_e4a?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Arquisoft/Loader_e4a&amp;utm_campaign=Badge_Grade)            | [![codecov](https://codecov.io/gh/Arquisoft/Loader_e4a/branch/master/graph/badge.svg)](https://codecov.io/gh/Arquisoft/Loader_e4a)               | Aplicacion de escritorio                                       |
| [Agents](https://github.com/Arquisoft/Agents_e4a)               | [![Build Status](https://travis-ci.org/Arquisoft/Agents_e4a.svg?branch=master)](https://travis-ci.org/Arquisoft/Agents_e4a)           | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f2f0d0b009384c8aba7deacb39b7b541)](https://www.codacy.com/app/Llambi/Agents_e4a?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Arquisoft/Agents_e4a&amp;utm_campaign=Badge_Grade)           | [![codecov](https://codecov.io/gh/Arquisoft/Agents_e4a/branch/master/graph/badge.svg)](https://codecov.io/gh/Arquisoft/Agents_e4a)               | http://ec2-54-149-62-135.us-west-2.compute.amazonaws.com:8081/ |
| [InicManager](https://github.com/Arquisoft/InciManager_e4a)     | [![Build Status](https://travis-ci.org/Arquisoft/InciManager_e4a.svg?branch=master)](https://travis-ci.org/Arquisoft/InciManager_e4a) | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f2f0d0b009384c8aba7deacb39b7b541)](https://www.codacy.com/app/Llambi/InciManager_e4a?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Arquisoft/InciManager_e4a&amp;utm_campaign=Badge_Grade) | [![codecov](https://codecov.io/gh/Arquisoft/InciManager_e4a/branch/master/graph/badge.svg)](https://codecov.io/gh/Arquisoft/InciManager_e4a)     | http://ec2-54-149-62-135.us-west-2.compute.amazonaws.com:8880/ |
| [InciDashboard](https://github.com/Arquisoft/InciDashboard_e4a) | ![Build Status](https://travis-ci.org/Arquisoft/InciDashboard_e4a.svg?branch=master) | ![Codacy Badge](https://api.codacy.com/project/badge/Grade/f2f0d0b009384c8aba7deacb39b7b541)                                                                                                                    | [![codecov](https://codecov.io/gh/Arquisoft/InciDashboard_e4a/branch/master/graph/badge.svg)](https://codecov.io/gh/Arquisoft/InciDashboard_e4a) | http://ec2-18-237-92-40.us-west-2.compute.amazonaws.com:8090/  |

## Authors originales

* Daniel Alba Muñiz (UO245188)
* José Luis Bugallo González (UO244702)
* Ignacio Escribano Burgos (UO227766)
* Daniel Duque Barrientos (UO245553)
* Rubén de la Varga Cabero (UO246977)
* David Lorenzo González (UO244795)
* Martín Peláez Díaz (UO236974)
* Laura Menéndez Pérez (UO244646)
* Fernando Palazuelo Ginzo (UO244588)

## Authors modificacion

* Pablo Amorin Triana (UO237060)
* Hugo Perez Fernandez (UO250708)
* Ivan Casielles Alvarez (UO251063)
* Mirza Ojeda Vieira (UO251443)
* Antonio Payá González(UO251065)
* Pablo Fernández Pérez (UO245015)
* Gonzalo Collada Vázquez (UO252066)
* Carlos Concheso Cubillas (UO237674)
* Paloma Sierra Bonet (UO232919)
* Pelayo Garcia Menendez (UO251765)

## Descripcion

Este es el proyecto conjunto de los 4 módulos utilizados. 

## Manual de uso

### Loader: Ejecucion

Para ejecutar la aplicacion se debe ir al directorio *ejecucion* y una vez ahi se dispondra de tres archivos .bat:

* *Help*: Para ver la ayuda de la aplicacion.
* *Info*: Para ver la informacion sobre la aplicacion.
* *Test*: Para realizar una ejecucion de la aplicacion.

Ademas para realizar una ejecucion de la aplicacion por uno mismo se debera ejecutar en la linea de comandos la siguiente instruccion:

	mvn -q exec:java -Dexec.mainClass="main.LoadAgents" -Dexec.args="Aqui iran los argumentos a usar"
	
	e.j.:mvn -q exec:java -Dexec.mainClass="main.LoadAgents" -Dexec.args="load src/test/resources/test.csv src/test/resources/test.xlsx"

### Agents: Datos Para Probar La Aplicación
  
  - Agente 1
    Login: 13864928P
    Password: 123456
    Kind: Person
    
  - Agente 2
    Login: 87654321B
    Password: 123456
    Kind: Person
    
  - Agente 3
    Login: 11223344C
    Password: 123456
    Kind: Person
   
### InciManager

#### Ejecucion

1- Descargar Apache Kafka de su página oficial.

  ->https://www.apache.org/dyn/closer.cgi?path=/kafka/1.0.1/kafka_2.11-1.0.1.tgz

2- Ejecutar Apache Zookeeper.

  ->bin\windows\zookeeper-server-start.bat config\zookeeper.properties

3- Ejecutar Apache Kafka.

  ->bin\windows\kafka-server-start.bat config\server.properties

4- Ejecutar eclipse desde la clase Application

5- Conectarse al localhost:8880

6- Introducir datos para loguearte

7- Consultar tus incidencias o crear una nueva

8- Si seleccionas crear una nueva, rellenas los datos y lo envias


# REST para crear una incidencia

{ 
	"login": "13864928P", 
	"password": "123456", 
	"kind": "Person", 
	"name": "nombreIncidencia2", 
	"description": "descripcionIncidencia", 
	"location": ["11.111111","-2.222222"], 
	"labels": "label1,label2,label3", 
	"moreInfo": ["adInfo1","adInfo2","adInfo3"], 
	"properties" : { 
		"key1":"value1", 
		"key2":"value2" 
	} 
}

### InciDashboard

#### Ejecucion

1. Arrancar [HSQLDB](https://sourceforge.net/projects/hsqldb/files/hsqldb/hsqldb_2_4/hsqldb-2.4.0.zip/download)
   * Para ello, acceder a la carpeta data/hsqldb/bin y lanzar el runServer.bat (o runServer.sh en caso de Linux/Mac).
2. Tener Apache Kafka. 
   * Instrucciones de instalación y despliegue en https://kafka.apache.org/quickstart.
2. Arrancar Apache Zookeeper desde directorio de Apache-kafka:
   * Mac/Linux: ``bin/zookeeper-server-start.sh config/zookeeper.properties``
   * Windows: ``bin\windows\zookeeper-server-start.bat config\zookeeper.properties``
3. Arrancar Apache Kafka desde directorio de Apache-kafka:
   * Mac/Linux: ``bin/kafka-server-start.sh config/server.properties``
   * Windows: ``bin\windows\kafka-server-start.bat config\server.properties``
4. Para arrancarlo todo y que funcione, se debe ejecutar el siguiente comando, estando situado en la carpeta InciDashboard_e4a:
``mvn spring-boot:run``
5. Para lanzar incidencias: En windows: bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic incidencia

```json
{ "agent":{ 
		"username": "xxxxx",
		"password": "xxxxx",
		"kind": "xxxx"
	},
	"inciName": "xxxxx",
	"location":{	
		"lat": "xxxxx",
		"lon": "xxxxx"
	},
	"tags": "xxxxx",
	"moreInfo": "xxxxx",
	"properties":{
		"propiedad1": "xxxx",
		"propiedad2": "xxxx"
	}
}
```

#### Usuarios para acceso

* User: hugo@gmail.com pass: 123456
* User: antonio@gmail.com pass: 123456
* User: pasadores@gmail.com pass: 123456
* User: mirza@gmail.com pass: 123456
* User: ivan@gmail.com pass: 123456


#### Pruebas de carga

Para la realización de las pruebas de carga se requiere el uso de [Gatling](https://gatling.io/). 
```shell
gatling.sh -s testGatling.scala
```

//TODO:


