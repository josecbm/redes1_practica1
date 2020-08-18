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

> ip 192.168.17.30 255.255.255.0 192.168.17.254

guardar

> save

### Maquina 3 

Para ver la direccion ip

> sh ip

Para agregar ip mascara de subred gateway

> ip 192.168.17.30 255.255.255.0 192.168.17.254

Para guardar

> save

### Maquina 4 

Para ver la direccion ip

> sh ip

Para agregar ip mascara de subred gateway

> ip 192.168.17.30 255.255.255.0 192.168.17.254

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

> ip address 192.168.17.1 255.255.255.0

> no sh

> exit

> interface FastEthernet0/1

> ip address 192.168.19.1 255.255.255.0

> no sh

> exit

> exit

Comando para guardar

> wr

Ver configuraciones 

> sh ip int br

### Topologia de la practica 
    
[this is the description](http://www.github.com)

This paragraph has some `variable` inline code.

```html
<p>A paragraph example</p>
```
```javascript
let num = Math.random();
```

![alt text](https://drive.google.com/file/d/1zCRsSm1aRvEozsgaGM_8KBWVfjjKIRH4/view?usp=sharing)


This is being * created * on a ** Friday ** ~~Saturday~~.
