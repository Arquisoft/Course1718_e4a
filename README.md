# Course1718_e4a

*Skeleton of Course1718_e4a project*

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

//TODO:


