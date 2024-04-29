# ControlHorarios

## Descripción


La aplicación web que se propone tiene como objetivo principal facilitar el registro y la asignación de horarios para empleados de una empresa o institución. Para ello, se utilizará el framework Angular junto con una librería de Gantt, lo que permitirá una interfaz dinámica e intuitiva para la gestión de los horarios.

El proceso de desarrollo se dividirá en varias etapas. En primer lugar, se diseñará y desarrollará la interfaz de usuario utilizando Angular, aprovechando sus capacidades para crear componentes reutilizables, estructura modular y gestión eficiente del estado de la aplicación. La interfaz estará diseñada de manera que sea fácil de entender y utilizar tanto para los administradores encargados de asignar los horarios como para los empleados que consultan sus propios horarios.

Una vez establecida la interfaz de usuario, se integrará una librería de Gantt que permita visualizar y gestionar los horarios de manera eficiente. Esta librería ofrecerá funcionalidades como la creación, modificación y eliminación de tareas (en este caso, turnos de trabajo), así como la capacidad de arrastrar y soltar para ajustar los horarios de manera intuitiva. Además, se implementarán características como la visualización de la carga de trabajo de cada empleado, la detección de conflictos de horarios y la generación de informes y estadísticas sobre la distribución del tiempo laboral.

Para garantizar la seguridad de los datos y la privacidad de los empleados, se implementarán medidas de autenticación y autorización, de modo que solo los usuarios autorizados puedan acceder y realizar cambios en los horarios. Se podrán establecer diferentes niveles de acceso, como administradores con control total sobre los horarios y empleados con permisos limitados para consultar su propio horario y solicitar cambios.
## Historias de Usuario 

### Empleado

- **HI-USA-001:** Como empleado, quiero poder solicitar mi horario para el próximo mes, eligiendo el tipo de turno que      prefiero, para tener mayor flexibilidad y comodidad en mi jornada laboral.
- **HI-USA-002:** Como empleado, quiero ver mi horario mensual en un formato de Gantt para tener una visión clara y estructurada de mis turnos de trabajo, facilitando así la planificación de mis actividades fuera del trabajo.
- **HI-USA-003:** Como empleado, quiero que la aplicación me indique claramente a qué sede pertenezco y a qué área de trabajo, para tener una referencia rápida de mi ubicación laboral.
- **HI-USA-004:** Como empleado, deseo tener la capacidad de solicitar vacaciones a través de la aplicación, indicando las fechas deseadas y asegurándome de que no haya conflictos con mi horario laboral, permitiéndome disfrutar de períodos de descanso sin afectar la operatividad del equipo.
- **HI-USA-005:** El empleado quiere solicitar vacaciones visualizando los días disponibles, facilitando la elección de fechas que se ajusten tanto a sus necesidades como a la disponibilidad de la empresa.
- **HI-USA-006:** Después de elegir mi turno deseado, la función de confirmación es rápida y eficiente, asegurando una respuesta inmediata para que pueda organizarme con anticipación.
- **HI-USA-007:** La aplicación me notifica vía correo electrónico sobre el veredicto de mi solicitud, que puede ser rechazado o aceptado, proporcionando una comunicación clara y oportuna sobre el estado de mi solicitud.


### Administrador

- **HI-USA-008:** Quiero gestionar y ajustar el número de empleados permitidos en cada tipo de turno, para garantizar una distribución equitativa de recursos y optimizar la asignación de tareas. 
- **HI-USA-009:** Deseo asignar periodos de training dentro del calendario de los empleados, para mejorar las habilidades y conocimientos del personal, contribuyendo al desarrollo profesional de manera planificada. 
- **HI-USA-010:** Deseo registrar a nuevos empleados en la aplicación y realizar cambios en sus horarios cuando sea necesario, para mantener actualizada la información del personal y adaptarla a las necesidades operativas.
- **HI-USA-011:** Deseo poder cargar información de forma masiva mediante archivos en formatos .xlsx, .json y/o .csv, para facilitar la gestión eficiente de grandes cantidades de datos y mantener la consistencia en la base de información.


### Super Administrador
- **HI-USS-012:** El super administrador se loguea, visualiza y selecciona la lista de todos los administradores y la región que administran, para llevar un control centralizado de las funciones administrativas.
- **HI-USS-013:** Si selecciona a un administrador, visualiza todos los empleados que este administra, permitiendo un seguimiento detallado de la gestión de personal por parte de cada administrador.
- **HI-USS-014:**  Quiero visualizar las jornadas de trabajo de cada empleado para determinar el mejor momento para sus vacaciones, facilitando la planificación y asegurando la continuidad operativa.
- **HI-USS-015:**  Quiero dar de alta nuevos usuarios administradores y otros tipos de usuarios para tener más apoyo en la administración de las distintas regiones, garantizando una gestión eficiente y escalable.
- **HI-USS-016:**  Quiero recibir alertas sobre posibles problemas de rendimiento o seguridad en la aplicación, para tomar medidas proactivas y mantener la estabilidad del sistema.
- **HI-USS-017:**  Necesito tener la capacidad de realizar copias de seguridad y restaurar datos en caso de pérdida o errores críticos, para asegurar la disponibilidad y la integridad de la información del sistema y garantizar la continuidad del servicio.

- 
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

### Diagrama de Actividades
<img width="280" alt="image" src="https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/377d7866-197e-40ad-a52f-66a11bba2dea">

### Diagrama de Clases
![DClases](https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/2e3c5974-5847-4914-a71e-a00603d8c7ea)


## Vistas

### Barra de navegación Empleado
- Botones: Inicio, Solicitudes, Gantt.
  <img width="302" alt="image" src="https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/3d86b9c7-57b1-42ff-b3db-0825721fb391">

### Barra de navegación Administrador
- Botones: Inicio, Gestión empleados, Solicitudes, Gantt.
  ![image](https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/a7e2bdf3-8aa7-433c-96e3-d931c02ea813)


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

![DC1](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc1.jpg)

![DC2](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc2.jpg)

![DC3](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc3.jpg)

![DC4](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc4.jpg)

![DC5](https://raw.githubusercontent.com/ABOK451/proyecto-control-horarios/main/documentacion/diagrama%20de%20componente/dc5.jpg)

Basándome en la información proporcionada, propongo un plan de iteraciones para el desarrollo del sistema de control de horarios:

### Iteración 1: Configuración del Entorno y Diseño de la Interfaz de Usuario
- Configurar el entorno de desarrollo con Angular.
- Diseñar la estructura de componentes y módulos de la interfaz de usuario.
- Implementar la autenticación básica para empleados, administradores y super administradores.
- Crear las páginas de inicio de sesión y página de bienvenida para cada tipo de usuario.

### Iteración 2: Implementación de Funcionalidades Básicas del Módulo de Empleado
- Desarrollar la funcionalidad para que los empleados puedan solicitar su horario para el próximo mes.
- Permitir a los empleados ver su horario mensual en formato de Gantt.
- Implementar la capacidad para que los empleados soliciten vacaciones a través de la aplicación.
- Añadir la funcionalidad para que los empleados puedan ver información sobre su sede y área de trabajo.

### Iteración 3: Implementación de Funcionalidades Básicas del Módulo de Administrador
- Desarrollar la funcionalidad para que los administradores gestionen y ajusten el número de empleados por turno.
- Permitir a los administradores asignar periodos de training dentro del calendario de los empleados.
- Implementar el registro de nuevos empleados y la capacidad de realizar cambios en sus horarios.

### Iteración 4: Integración de la Librería de Gantt y Mejoras en la Interfaz de Usuario
- Integrar la librería de Gantt para visualizar y gestionar los horarios de manera eficiente.
- Mejorar la interfaz de usuario para que sea más intuitiva y fácil de usar.
- Añadir características como la visualización de la carga de trabajo de cada empleado y la detección de conflictos de horarios.

### Iteración 5: Implementación de Funcionalidades del Módulo de Super Administrador
- Desarrollar la funcionalidad para que el super administrador pueda visualizar y seleccionar la lista de todos los administradores y las regiones que administran.
- Permitir al super administrador gestionar los usuarios y sus permisos, incluyendo la creación de nuevos usuarios administradores.

### Iteración 6: Refinamiento y Pruebas
- Realizar pruebas exhaustivas del sistema para detectar y corregir errores.
- Optimizar el rendimiento y la seguridad del sistema.
- Mejorar la documentación del proyecto, incluyendo el manual de instalación y casos de prueba.

### Diagrama Entandares de base de datos
![DBase](https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/9ad246ad-1a6f-4ab0-9668-bedf16e67142)


### Explicación del Modelo

- `Administrador`: Almacena información sobre los administradores del sistema.
- `Empleado`: Contiene datos de los empleados.
- `SuperAdmin`: Almacena información sobre los superadministradores.
- `Area`: Representa las áreas de trabajo en la empresa.
- `Turno`: Contiene información sobre los turnos de trabajo.
- `Contrato`: Describe los detalles de los contratos laborales.

### Consideraciones del Modelo

- Cada empleado puede tener asociado un único turno de trabajo.
- Cada empleado tiene un único administrador asociado.
- Cada empleado pertenece a un área específica.
- Los administradores y superadministradores pueden gestionar múltiples empleados.
- Los empleados pueden solicitar vacaciones y turnos de trabajo.
- Los contratos contienen información sobre los días laborales, días de descanso y horas por día.

## Manual de Instalación
  - https://drive.google.com/drive/folders/13ea2IMSp6LadQ8AzyaKcv9Fye6yTEtRI?usp=drive_link
## Casos de Pruebas
- https://drive.google.com/drive/folders/1O5lQufb_uz0nobFIUe_qKMd_WQk1UQkI?usp=drive_link
## Testeo
- https://docs.google.com/document/d/1R_7I0qQZ1ZgCtb7MkD25DTOzAGaf0YHmcfvWZ9a3qYs/edit?usp=sharing
