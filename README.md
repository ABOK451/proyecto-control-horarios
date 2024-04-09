# ControlHorarios

## Descripción
Aplicación web para el registro y asignación de horarios de empleados, utilizando Angular y una librería de Gantt.

## Historias de Usuario 

### Empleado

- **HI-USE-001:** Solicitar horario mensual.
- **HI-USE-002:** Visualizar horario mensual en formato Gantt.
- **HI-USE-003:** Confirmación rápida de solicitud de horario.
- **HI-USE-004:** Solicitar vacaciones.
- **HI-USE-005:** Acceder al historial de horarios anteriores.
- **HI-USE-006:** Visualizar y gestionar documentos personales.

### Administrador

- **HI-USA-001:** Gestionar número de empleados por turno.
- **HI-USA-002:** Asignar periodos de training a empleados.
- **HI-USA-003:** Registrar nuevos empleados y cambios de horario.
- **HI-USA-004:** Generar horario mensual automáticamente.
- **HI-USA-005:** Visualizar horarios de empleados en formato Gantt.

### Super Administrador

- **HI-USS-001:** Visualizar lista de administradores y regiones.
- **HI-USS-002:** Ver empleados de cada administrador.
- **HI-USS-003:** Visualizar jornadas de trabajo de empleados.
- **HI-USS-004:** Dar de alta nuevos administradores y usuarios.
- **HI-USS-005:** Realizar copias de seguridad y restaurar datos.

## Análisis de la Solución
### Requerimientos Funcionales - Integradora 2024

#### Módulo de Empleado:

1. El sistema debe permitir a los empleados solicitar su horario para el próximo mes, eligiendo el tipo de turno deseado durante la última semana de cada mes.
2. La aplicación debe mostrar a cada empleado su horario mensual en formato de Gantt, proporcionando una visualización clara de los turnos de trabajo.
3. Después de solicitar un turno, el sistema debe confirmar la elección de manera rápida y eficiente. Además, se enviará una notificación por correo electrónico con la opinión de la solicitud.
4. Los empleados deben tener la capacidad de solicitar vacaciones a través de la aplicación, indicando las fechas deseadas y asegurándose de que no haya conflictos con el horario laboral.
5. La aplicación debe mostrar visualmente los días disponibles para solicitar vacaciones, facilitando la elección de fechas por parte del empleado.
6. Los empleados deben poder acceder a un historial de sus horarios anteriores para referencia y planificación personal.

#### Módulo de Administrador:

1. Los administradores deben tener la capacidad de gestionar y ajustar el número de empleados permitidos en cada tipo de turno para garantizar una distribución equitativa de recursos.
2. Los administradores deben poder asignar periodos de training dentro del calendario de los empleados para mejorar sus habilidades y conocimientos.
3. Los administradores deben poder registrar nuevos empleados en la aplicación y realizar cambios en sus horarios cuando sea necesario para mantener actualizada la información del personal.
4. La aplicación debe generar automáticamente los horarios mensuales de los empleados basándose en el contrato y turno elegido, evitando asignar días de trabajo o descanso en días de training o vacaciones.
5. Los administradores deben tener la capacidad de visualizar los horarios de los empleados en formato de Gantt mediante una librería actualizada.

#### Módulo de Super Administrador:

1. El super administrador debe poder visualizar y seleccionar la lista de todos los administradores y las regiones que administran para un control efectivo.
2. Al seleccionar a un administrador, el super administrador debe poder visualizar todos los empleados que administra dicho administrador.
3. El super administrador debe poder visualizar las jornadas laborales de cada empleado para determinar el mejor momento para sus vacaciones.
4. El super administrador debe tener la capacidad de dar de alta nuevos usuarios administradores y otros tipos de usuarios.


## Diagrama de Casos de Uso

### Actores

1. SuperAdmin
2. Admin
3. Empleado

![DCU1](https://github.com/ABOK451/proyecto-control-horarios/blob/main/documentacion/diagrama%20casos%20de%20uso/imagen_2024-04-09_000129415.png)

![DCU2](https://github.com/ABOK451/proyecto-control-horarios/blob/main/documentacion/diagrama%20casos%20de%20uso/imagen_2024-04-09_000151169.png)

![DCU3](https://github.com/ABOK451/proyecto-control-horarios/blob/main/documentacion/diagrama%20casos%20de%20uso/imagen_2024-04-09_000204959.png)

## Vistas

### Barra de navegación Empleado
- Botones: Inicio, Solicitudes, Gantt.

### Barra de navegación Administrador
- Botones: Inicio, Gestión empleados, Solicitudes, Gantt.

### INICIO
- Logotipo y lema de la aplicación.

### INICIO DE SESION
- Campos para correo electrónico y contraseña.

### PÁGINA DE BIENVENIDA
- Barra de navegación Empleado y mensaje de bienvenida.

### EMPLEADO

#### SOLICITUD DE EMPLEADO HORARIO 
- Ciudad y departamento calculados automáticamente.
- Campo para descripción opcional.
- Visualización de turnos disponibles.

#### SOLICITUD DE EMPLEADO VACACIONES 
- Ciudad y departamento calculados automáticamente.
- Campos para fechas de vacaciones.

### SUPERADMIN / ADMIN / ROOT

#### CRUD EMPLEADO 
- Formulario con información personal y horarios.

#### CRUD AREA 
- Formulario para añadir áreas de trabajo.

#### CRUD CIUDAD / SEDE 
- Formulario para añadir ciudades.

#### CRUD USUARIOS
- Formulario para añadir usuarios y asignar permisos.

#### CRUD ACTIVIDADES VAC/TRAINING/WORKDAY 
- Formulario para asignar horarios de trabajo y training.

#### Grafico de Gantt
- Generado para cada usuario seleccionado.

#### SOLICITUDES VAC/TURNO 
- Tabla de solicitudes con botones de aceptar y rechazar.

#### CARGA MASIVA 
- Vista para cargar archivos de datos.


## Modelo de la base de datos

- **Administrador**
  - NombreAdmin: String
  - CorreoAdmin: String
  - Contrasena: String
  - Region: String
  - Root: String

- **Area**
  - NombreArea: String
  - Descripcion: String

- **Contratos**
  - TipoContrato: String
  - DiasTrabajados: Number
  - DiasDescansados: Number
  - HorasPorDia: Number
  - TurnosContrato: Array

- **Departamento**
  - NombreDepartamento: String
  - Direccion: 
    - Numero: String
    - Calle: String
    - Colonia: String
    - Cp: String

- **Empleado**
  - Nombre: String
  - AppE: String
  - ApmE: String
  - FechaNac: Date
  - Correo: String
  - Contrasena: String
  - Region: String
  - AreaTrabajo: String
  - Departamento: String
  - Contrato: String
  - TurnoActual: 
    - Inicio: String
    - Fin: String
  - HorarioTraining: 
    - Fecha: Date
    - HoraInicial: String
    - HoraFinal: String
  - NombreAdmin: String
  - FechaDeIngreso: Date

- **HistorialHorario**
  - NombreEmpleado: String
  - FechaInicio: Date
  - FechaFin: Date

- **Sede**
  - Region: String
  - Pais: String

- **SolicitudHorario**
  - NombreEmpleado: String
  - NombreAdmin: String
  - Contrato: String
  - TurnoSolicitado: 
    - Inicio: String
    - Fin: String
  - EstadoSolicitud: String
  - Correo: String

- **SolicitudVacaciones**
  - NombreEmpleado: String
  - FechaSolicitud: 
    - FechaInicioVacaciones: Date
    - FechaTerminoVacaciones: Date
  - EstadoSolicitud: String
  - Descripcion: String

- **Turno**
  - NombreTurno: String
  - HoraFinal: Date
  - HoraInicio: Date
 
## Diagrama de Componentes
## Diagrama de Componentes

![DC1](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc1.jpg)

![DC2](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc2.jpg)

![DC3](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc3.jpg)

![DC4](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc4.jpg)

![DC5](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc5.jpg)

  

