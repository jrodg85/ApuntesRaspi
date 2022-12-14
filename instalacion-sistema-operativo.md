# Instalacion del Sistema operativo en la tarjeta SD

## Pendiente puesta a punto de la tarjeta Micro SD.

---

# Instalación de SO Raspbian en la tarjeta SD

### Desde un Pc Windows

- Se procede a la instalación de la aplicación Raspberry Pi Imager
  - Se puede descargar la aplicación en la siguiente URL https://www.raspberrypi.com/software/.

- Se procede a su Instalación.

- Se procede a insertar la tarjeta Micro SD que se usará en la "Raspi" en el pc.

- Se procede a ejecutar Raspberry Pi Imager

![Seleccionar aplicación](./assets/001-ejecucion-raspberry-pi-imager.png)

- Aparecerá la pantalla de la aplicación.

![Inicio de Raspberry Pi Imager](./assets/002-inicio-aplicacion-raspberry-pi-imager.png)

- Seleccionamos ***CHOOSE OS*** $\rightarrow$ ***Raspberry Pi OS (other)*** $\rightarrow$ ***Raspberry Pi OS Full (32-bit)***.

![Selección de Sistema Operativo](./assets/003-seleccion-de-sistema-operativo.png)

- A continuación, nos devuelve a la pagina principal de la aplicación con el SO seleccionado.


![SO cargado](./assets/004-SO-cargado-elegimos%20almacenamiento.png)

- Seleccionamos ***CHOOSE STOREAGE*** $\rightarrow$ ***Mass Storage Device USB Device - 32.0GB***

![Seleccionando Unidad](./assets/005-seleccion-tarjeta-micro-SD.png)


- Volverá a la pantalla principal con la unidad USB (donde se encuentra la tarjeta micro SD)

![Tarjeta SD cargada](./assets/006-pulsamos-engranaje.png)

- Procedemos a hacer click en el engranaje.

![Configuracion de carga](./assets/007-configuracion-para-instalacion-01.png)

- Procedemos a realizar las siguiente configuración:
  - Set Hostname.
  - Enable SSH.
    - Use Password authentication.
  - Set Username and password.
    - Escribimos User y password que tendrá la Raspberry.
  - Configure wireless LAN:
    - Wireles LAN country $\rightarrow$ ES
  - Set locale setting:
    - Para Time Zone yo uso $\rightarrow$ Etc/UTC.
    - Para keyboard layout seleccionamos $\rightarrow$ es.
- Pulsamos el botón $\rightarrow$ SAVE.
- Pulsamos el botón $\rightarrow$ WRITE.

![Pulsamos Write](./assets/008-pulsamos-write.png)

- Diremos que si a la advertencia ya que eliminaremos todos los datos de la tarjeta SD.

- Se procede a la instalación de Raspbian en el dispositivo SD.

![Carga del SO en la SD](./assets/009-proceso-de-carga-en-SD.png)

- Tras la instalación, la aplicación procede a comprobar la correcta instalación del SO en la tarjeta SD.

![Verificación de la correcta instalación del SO en la SD](./assets/010-verificaci%C3%B3n.png)

- La instalación del SO en la SD habrá finalizado.

- Se procede la configuración para poder arrancar el dispositivo.
  - Se extrae la tarjeta SD del PC y se procede a su colocación en la Raspberry.

  ***insertar foto aqui***


- Se procede a conectar lo siguiente:
  - Entrada USB-C $\rightarrow$ fuente de alimentación
  - Entrada USB 2.0 $\rightarrow$ Teclado y ratón (en nuestro caso es inalámbrico y solo es necesario un puerto USB).
  - Salida Micro-HDMI $\rightarrow$ monitor a través de cable HDMI y cable de trancisión HDMI hembra a micro-HDMI macho.

  ***Insertar foto aqui***

- Procedemos a su encendido.
  - Durante el encendido de este... si a los **3 minutos** la Raspberry parece haberse quedado colgada, es decir ves la pantalla en negro durante al menos **durante esos 3 minutos, nunca menos**.
    - Se procede a un apagado y encendido manual, esta acción posiblemente la tengas que repetir 3 o 4 veces. Si hubiera que hacer una quinta vez, mejor inicializar la instalación de 0 de la tarjeta SD.

- En nuestro caso, al usar una pantalla de Tv de 45", es necesario cambiar la configuración de la pantalla para ponerla mas acorde a la distancia de la pantalla.
  - Para ello, haremos click en el logotipo de Raspberry (arriba a la izquierda por defecto) $\rightarrow$ Preferences $\rightarrow$ Raspberry Pi Configuration.


  ***insertar imagen aqui***


- Ahora configuraremos la resolución para VNC cuando el monitor no esta conectado.
  - En la pestaña de Display, seleccionaremos el desplegable de Headless Resolution: $\rightarrow$ 1920x1080.

    ***insertar imagen aqui***

- Activaremos VNC para su posterior conexión a través de este sistema.
  - Seleccionamos en la pestaña interfaces y activaremos el check de VNC.


    ***insertar imagen aqui***


- Por ultimo, en Raspberry Pi Configuration, procederemos a la pestaña Localisation y comprobaremos todos los apartados. En mi caso, no tenían concordancia con lo indicado previamente se habia cargado durante la instalación de Raspbian en la SD.
  - Locale $\rightarrow$ Set Locale...
    - Language $\rightarrow$ es (Spanish).
    - Country $\rightarrow$ ES (Spain).
    - Character set $\rightarrow$ ISO-8859-1.
    - Aceptamos.

    ***insertar imagen aqui***

  - Timezone $\rightarrow$ Set Timezone...
    - Area: $\rightarrow$ UTC.
    - Location: $\rightarrow$ en blanco.
    - Aceptamos.

    ***insertar imagen aqui***

  - Keyboard: $\rightarrow$ Set Keyboard...
    - Model: $\rightarrow$ Generic 105-key PC (intl.).
    - Layout: $\rightarrow$ Spanish.
    - Variant: $\rightarrow$ Spanish.
    - Aceptamos.

    ***Insertar Imagen Aqui***

  - Wireless LAN Country $\rightarrow$ Set WLAN Country...
    - Country: $\rightarrow$ ES Spain.
    - Aceptamos.

    ***Insertar Imagen Aqui***

  - Aceptamos

- Pedirá el reinicio de la Raspberry, le diremos que si para que todas las configuraciones tengan efecto.

***Insertar foto***

- Procedemos a su reinicio.

- Una vez reiniciado el sistema procedemos a ver la configuración de VNC para ello haremos click en el icono de VNC situado en la parte superior derecha.

***insertar imagen icono aqui***

- Nos aparecerá una ventana en la que nos indicará la manera de conexión a través de VNC, en nuestro caso a través de la dirección ip 192.168.1.71, dirección IP de la LAN a la cual la Raspberry esta conectada.

***Insertar foto***

- Procederemos al apagado de la Raspberry y a su instalación en su emplazamiento definitivo sin necesidad de conectar teclado ni salida micro-HDMI.

- En nuestro caso hemos conectado un cable de red para hacer después la conexión con el router de manera física.

***Insertar foto***

---



