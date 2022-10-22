---
weight: 3
bookFlatSection: true
title: "Cliente --> Servidor"
---

# Comunicación de un cliente con un servidor

En esta página vamos a intentar explicar el proceso por el cual se comunica un cliente con un servidor.

La *arquitectura cliente-servidor* o *modelo cliente-servidor* es un protocolo de comunicación a través de una red (como puede ser Internet) en el que las tareas se reparten entre los proveedores de recursos o servicios, llamados **servidores**, y los demandantes, llamados **clientes**.

Un cliente realiza peticiones a otro programa, el servidor, quien le da respuesta.

En este caso, para explicar cómo se realiza la comunicación, vamos a centrarnos en el proceso de carga de una página web.

Es importante mencionar que gran parte de los servicios de Internet obedecen a la *arquitectura cliente-servidor*. El servidor web pone a disposición del cliente los sitios web, a los cuales se accede a través del navegador. Es el servidor el que aloja los datos que el cliente (navegador) solicita.

### Conceptos importantes:
>> **Cliente**: dispositivo conectado a Internet (por ejemplo, un ordenador conectado a la red Wi-Fi o un teléfono conectado a la red de telefonía móvil) y el software que se encuentra disponible y permite acceder a Internet (normalmente, un navegador web).

>> **Servidor**: computador que almacena páginas web, sitios o aplicaciones.

>> **TCP/IP: Protocolo de Control de Transmisión y Protocolo de Internet**, protocolos de comunicación que definen cómo deben viajar los datos a través de la web.

>> **DNS**: servidores del **Sistema de Nombres de Dominio**, podríamos definirlos como una libreta de direcciones de sitios web. Cuando escribes una dirección web en el navegador, normalmente un dominio (como *www.google.es*), el DNS traduce ese nombre de dominio a su dirección IP para averiguar en qué servidor vive el sitio web y así enviar los mensajes HTTP al lugar correcto.

>> **HTTP**: Protocolo de Transferencia de Hipertexto, es un protocolo de aplicación que define cómo se comunican clientes y servidores.

## ¿Qué ocurre, entonces?
Cuando escribes una dirección web (o dominio) en el navegador:

1. El navegador va al servidor DNS y encuentra la dirección real del servidor donde está alojado el sitio web.
2. El navegador envía un mensaje de petición HTTP al servidor, pidiéndole que envíe una copia de la página web para el cliente. Este mensaje y todos los datos enviados entre el cliente y el servidor, se envían a través de la conexión a Internet usando TCP/IP.
3. Siempre que el servidor apruebe la solicitud del cliente, el servidor comenzará a enviar los archivos de la página web al navegador como una serie de pequeños trozos llamados paquetes de datos.
4. El navegador reúne los pequeños trozos, forma un sitio web completo y te lo muestra.

## Ejemplo gráfico

{{< mermaid>}}
flowchart LR
    id1(Cliente - Navegador)-->id2(DNS)
    id2-- dirección IP -->id1
    id1-->id3{{Internet}}-->id4[(Servidor)]
{{< /mermaid >}}

Una vez aprobada la solicitud:
{{< mermaid>}}
flowchart LR
    id4[(Servidor)]-->id3{{Internet}}-->id1(Cliente - Navegador)
{{< /mermaid >}}