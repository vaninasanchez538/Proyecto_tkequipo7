Informatorio Etapa 2
Desarrollo Web 

Proyecto Tkinter
"Aplicación de Agenda de turnos"

Este proyecto es una aplicación de escritorio construida en Python con la librería Tkinter para gestionar turnos de distintos servicios simulando el uso por parte de un usuario. 
Tiene las siguientes funciones disponibiles:

- Ver los servicios disponibles.
- Reservar turnos en horarios definidos.
- Ver los turnos reservados.
- Cancelar un turno previamente agendado.
- Ver los créditos del equipo de desarrollo.

📁 Estructura y Lógica del Código
El código está dividido en tres partes principales: modelos, datos y usuario, e interfaz gráfica.

1. 📦 Modelos (Clases principales)

Usuario -> Representa al usuario que utiliza la app. Guarda sus datos y los turnos reservados.
Métodos: reservar_turno(turno): agrega un turno a su lista.

Servicio -> Representa un servicio (ej. "Musicoterapia", "Odontología").
Atributos: id, nombre, duracion.

Turno -> Representa un turno agendado con información de fecha, servicio, cliente y estado.
Tiene una representación personalizada con __str__.

2. 📋 Datos simulados

Lista de servicios precargados (servicios) que se pueden reservar.
Usuario ficticio ya “logueado” (usuario_actual).

3. 🖼️ Interfaz gráfica con Tkinter
Toda la interfaz es gestionada por la clase AppTurnos. Al iniciar, se muestra un menú principal con botones para acceder a distintas funcionalidades.

Funcionalidades disponibles:

mostrar_servicios() -> Muestra los servicios disponibles en una ventana secundaria.
abrir_reserva()     -> Abre un formulario para reservar turnos. Permite: -> Elegir un servicio (desplegable).
                                                                         -> Elegir fecha (con calendario).
                                                                         -> Elegir hora (bloques de 30 minutos entre 8-12 y 14-18).
                                                                         -> Validar que no haya turnos duplicados ni pasados ni en domingo.
                                                                         -> Ingresar nombre y apellido para confirmar.
                                                                         -> Guardar el turno en el usuario.

mostrar_turnos()   -> Lista todos los turnos que el usuario tiene agendados.
cancelar_turno()   -> Permite seleccionar un turno reservado y eliminarlo de la lista.
mostrar_creditos() -> Muestra una ventana con los nombres del equipo desarrollador.

🛠️ Requisitos
Python 3.x

Librerías:
tkinter
tkcalendar (instalable con pip install tkcalendar)

Integrantes del equipo 7:

Antúnez, Pablo
Avanzatti, Diego Gabriel
Criscueli, Eduardo Ezequiel
Fernández, Ezequiel Jesús
Salas, Gabriel Leonardo
Sánchez, Vanina
Viton, Eliana 


 
