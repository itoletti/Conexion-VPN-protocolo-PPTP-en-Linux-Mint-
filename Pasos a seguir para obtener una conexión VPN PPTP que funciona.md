# Conexion-VPN-protocolo-PPTP-en-Linux-Mint-
Solución para conectar VPN con protocolo PPTP en Linux Mint 20.3
Al intentar realizr una conexion con la VPN del trabajo en el equipo con linux Mint 20.3 encotre algunos problemas que pude sortear hasta que logre que funcionara.
En la barra de tareas en el area de Notificaciones en el icono de Centro de Redesla opcion Conexiones VPN mas adelante cuando pude crear una conexion VPN me aparecia grisada 
la opcion Configurar VPN... y tampoco con la conexion creada me permitia realizar la conexion ademas de que no me indicara ningun error.
Para realizar la conexion a la VPM segui las instrucciones que indican algunos sitios
  - desde el menu Inicio|Centro de Control seleccionar de Internet y Red la opcion Configuracion de red avanzada (ver fig 1)
  - en la ventana emergente seleccionar el boton + en la parte inferior derecha de la ventana que me permite agregar una nueva conexion (ver fig 2)
  - en la lista desplegabel de la nueva vebtana emergente seleccionar la opcion VPN Protocolo de túnel punto a punto (PPTP) (ver fig 2)
  - seleccionar el boto Crear...
  - En la ventana emergente de creación de la VPN agregar informacion a los campos (ver fig 3)
      - Nombre de la conexion: dandole el nombre que se la identificara luego en la lista de conexiones VPN en el Centro de Redes
      - Pasarela: indicar la url o nombre del servidor de VPN (vpn.nombre.com.ar)
      - Usuario: el usario para la conexion 
      - Password: la passwd del usuario de la conexion
      - Dominio de red: no es necesario agragar info alli
  - Seleccionar el boton Avanzado... de alli solo hacer los siguientes cambios (ver fig 4)
      - Marcar Usar cifrado punto a punto (MPPE)
      - en la lista desplegable seleccionar 128-bit (mas seguro)
      - en el cuadro Permitir los siguientes métodos de autenticacion: aparecen solo dos opciones habilitadas para modificar MSCHAP y MSCHAPv2, solo dejar marcado MSCHAPv2
      . dejar las demas opciones como estan por defecto y dar al boton Aceptar
  - darle al boton Guardar de la ventana Editando... donde se esta creando la conexion Nueva

Con esto ya apareceria en la barra de estado en la seccion notificaciones dentro del Cenrto de redes, la cuenta creada (ver fig 5 u fig 6) y podemos indicar desde alli que se conecte, ademas de poder ver alli la opcion de Configurar VPN... (habilitada para poder realizar modificaciones) 

