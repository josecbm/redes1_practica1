# redes1_practica1

## Carnet: 201504231
## Jose Carlos Bautista Mazariegos
### Maquina 1 (virtual)

Para ver la direccion ip del dispositivo
> ifconfig
Comando para agregar ip , mascara de subred y gateway

> sudo ifconfig eth0 192.168.17.15 netmask 255.255.255.0

> sudo route add default gw 192.168.17.254 eth0

### Maquina 2 

Para ver la direccion ip
> sh ip

Para agregar ip mascara de subred gateway

> ip 192.168.11.30 255.255.255.0 192.168.11.254

guardar

> save

### Maquina 3 

Para ver la direccion ip

> sh ip

Para agregar ip mascara de subred gateway

> ip 192.168.13.30 255.255.255.0 192.168.13.254

Para guardar

> save

### Maquina 4 

Para ver la direccion ip

> sh ip

Para agregar ip mascara de subred gateway

> ip 192.168.11.30 255.255.255.0 192.168.11.254

Para guardar

> save

### Router
Inicio entrar a la configuracion de la terminal

> configure terminal 

> line console 0

> no exec-timeout

> end

wr


## Configurar Router

> conf terminal 

> interface FastEthernet0/0

> ip address 192.168.11.1 255.255.255.0

> no sh

> exit

> interface FastEthernet0/1

> ip address 192.168.13.1 255.255.255.0

> no sh

> exit

> exit

Comando para guardar

> wr

Ver configuraciones 

> sh ip int br

### Topologia de la practica 
    
![topologia](https://user-images.githubusercontent.com/8570475/90991123-2052a980-e564-11ea-80dc-699d9296223d.png)


![vm](https://user-images.githubusercontent.com/8570475/90991260-ffd71f00-e564-11ea-9912-b05e4fbb4155.png)


![ping_ma1_ma2](https://user-images.githubusercontent.com/8570475/90991276-12e9ef00-e565-11ea-89ef-e3e0b044e3de.png)



### Pruebas y configuraciones

### Glosario

Gns3: Es un software utilizado por cientos de miles de ingenieros de redes a nivel mundial para emular, configurar, probar y
solucionar problemas de redes virtuales y reales. Le permite ejecutar una pequeña topología que consta de solo unos
pocos dispositivos en su computadora portátil, a aquellos que tienen muchos dispositivos alojados en múltiples
servidores o incluso alojados en la nube.

Router: El router se encargaría de ir asignando IPs dentro del rango que le indiquemos a los diferentes equipos que se vayan
conectando. Esto hará imposible que por confusión dos equipos tengan la misma IP entrando en conflicto.

VPC: Es el acronimo de virtual PC, en el proyecto estas haran de simulación de una computadora.

Virtual machine:  Software que simula un sistema de computación y que los procesos que ejecuta están limitados por los recursos y
abstracciones proporcionados por ellas. Estos procesos no pueden escaparse de esta "computadora virtual"

Ip : Es una serie de condiciones y reglas sobre las cuales se maneja todo el espectro comunicacional entre computadoras en
la red.


 Mascara de red: Es una combinación de bits que sirve para delimitar el ámbito de una red de ordenadores.1Su función es indicar a los
dispositivos qué parte de la dirección IP es el número de la red, incluyendo la subred, y qué parte es la correspondiente
al host.

Gateway: Es el dispositivo que actúa de interfaz de conexión entre aparatos o dispositivos, y también posibilita compartir recursos
entre dos o más ordenadores.

DHCP es un componente crítico, en tanto que en redes cableadas e inalámbricas, y mixtas, son varios los dispositivos
que se tienen que conectar de forma simultánea y, por lo tanto, del protocolo DHCP depende que se puedan mantener
las conexiones de forma estable.

Tiny Core Linux: TCL, es un sistema operativo minimalista centrado en proveer un sistema base con el núcleo Linux, BusyBox, FLTK y otro
software minimalista desarrollado por Robert Shingledecker. La distribución es especialmente notable por su reducido
tamaño (de 11 a 16 megabytes) y su minimalismo, y posee un repositorio que contiene más de 3200 extensiones

UTP El par trenzado sin blindaje (UTP) es un tipo generalizado de cable de cobre. Su nombre proviene del acrónimo inglés
de Unshielded Twister Pair, o par trenzado sin apantalla.

Puertos de acceso:  Los puertos de acceso pertenecen a un solo VLA N y llevan el tráfico en un solo VLA N solamente.

Puertos troncales: Los puertos troncales, llevan generalmente el tráfico de los VLAN múltiples y por abandono será el miembro de todos
los VLAN configurados en el Switch.
