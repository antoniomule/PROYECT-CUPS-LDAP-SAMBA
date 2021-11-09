# PROYECT CUPS + LDAP + SAMBA
 Proyecto final de grado Administración de sistemas informáticos en Red.

¿POR QUE LA NECESIDAD DE ÉSTE PROYECTO?

Para comenzar este proyecto tendremos que empezar emulando y explicando la tipología de red que
encontramos en el departamento de informática de nuestro grado de Administración de sistemas en red,
del servidor Servus.inf y del departamento de profesores.
Disponemos de una impresora de red Brother del departamento, actualmente esta impresora está
conectada directamente a la red por lo cual, cualquier dispositivo que se encuentre dentro de esta red,
podrá usar ésta impresora, ya sea desde un portátil de cualquier alumno de 2º o por cualquier
alumno/profesor que esté conectado ya sea por un ordenador dentro del dominio Servus.inf o fuera de
éste dominio, ya que tanto los alumnos como los profesores disponen de una cuenta global que se
autentica contra el servicio LDAP de Servus. Aquí radica el problema, ésta impresora no puede ser
gestionada directamente ya que está conectada a la red de forma independiente por lo cual cualquier
dispositivo puede usar esta impresora e imprimir como le plazcla, ya que al ser independiente al
servidor Servus.inf, no necesita autentificación ni autorización para ser utilizada.
Este proyecto consiste en que, gestionaremos mediante el servicio de impresión CUPS que se
encontrará en Servus.inf, y que sólo los usuarios que se encuentren dentro del dominio como por
ejemplo los profesores sean los veneficiarios de esta impresora.
Tendremos que cambiar la tipología de la red, y tendremos que conectar esa impresora Brother
directamente al servidor, mediante USB, por ejemplo (Dependiendo de la impresora puede usarse otro
tipo de conexión).
Emularé el servidor Servus.inf y las estaciones de trabajo usadas por los alumnos/profesores que se
autentican mediante LDAP y mediante el servidor CUPS gestionaremos la autorización y gestión de la
impresora Brother del departamento para que sólo pueda ser usada por los profesores.
Una vez sabemos esto, comencemos..