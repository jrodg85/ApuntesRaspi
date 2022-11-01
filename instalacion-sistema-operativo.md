# Instalacion del Sistema operativo en la tarjeta SD

## Desde un Pc Windows

- Se procede a la instalacion de la aplicacion Raspberry Pi Imager
  - Se puede descargar la aplicación en la siguiente URL https://www.raspberrypi.com/software/.

- Se procede a su Instalación.

- Se procede a insertar la tarjeta Micro SD que se usará en la "Raspi" en el pc.

- Se procede a ejecutar Raspberry Pi Imager

![Seleccionar aplicacion](./assets/001-ejecucion-raspberry-pi-imager.png)

- Aparecerá la pantalla de la aplicación.

![Inicio de Rasberry Pi Imager](./assets/002-inicio-aplicacion-raspberry-pi-imager.png)

- Seleccionamos ***CHOOSE OS*** $\rightarrow$ ***Raspberry Pi OS (other)*** $\rightarrow$ ***Raspberry Pi OS Full (32-bit)***.

![Selección de Sistema Operativo](./assets/003-seleccion-de-sistema-operativo.png)

- A continuacion nos devuelve a la pagina principal de la aplicacion con el SO seleccionado.


![SO cargado](./assets/004-SO-cargado-elegimos%20almacenamiento.png)

- Seleccionamos ***CHOOSE STOREAGE*** $\rightarrow$ ***Mass Storage Device USB Device - 32.0GB***

![Seleccionando Unidad](./assets/005-seleccion-tarjeta-micro-SD.png)


- Volverá a la pantalla principal con la unidad USB (donde se encuenta la tarjeta micro SD)

![Tarjeta SD cargada](./assets/006-pulsamos-engranaje.png)

- Procedemos a hacer click en el engranaje.

![Configuracion de carga](./assets/007-configuracion-para-instalacion-01.png)

- Procedemos a realizar las siguiente configuración:
  - Set Hosname.
  - Enable SSH.
    - Use Password authentication.
  - Set Username and password.
    - Escribimos User y password que tendrá la raspberry.
  - Configure wireless LAN:
    - Wireles LAN country $\rightarrow$ ES
  - Set locale setting:
    - Para Time Zone yo uso $\rightarrow$ Etc/UTC.
    - Para keyboard layout seleccionamos $\rightarrow$ es.
- Pulsamos el boton $\rightarrow$ SAVE.
- Pulsamos el boton $\rightarrow$ WRITE.

![Pulsamos Write](./assets/008-pulsamos-write.png)

- Diremos que si a la advertencia ya que eliminaremos todos los datos de la tarjeta SD.

- Se procede a la instalacion de Raspbian en el dispositivo SD.

![Carga del SO en la SD](./assets/009-proceso-de-carga-en-SD.png)

- Tras la instalación, la aplicación procede a comprobar la correcta instalación del SO en la tarjeta SD.

![Verificación de la correcta instalacion del SO en la SD](./assets/010-verificaci%C3%B3n.png)

- La instalacion del SO en la SD habra finalizado.

- Se procede la configuracion para poder arrancar el dispositivo.
  - Se extrae la tarjeta SD del PC y se procede a su colocación  bvh  en la Raspberry.

- Se procede a conectar lo siguiente:
  - Entrada USB-C $\rightarrow$ fuente de alimentacion
  - USB 2.0 $\rightarrow$ Teclado y ratón (en nuestro caso es inalambrico y solo es necesario un puerto USB).
  - Micro-HDMI $\rightarrow$ monitor a traves de cable HDMI.

- Procedemos a su encendido.
