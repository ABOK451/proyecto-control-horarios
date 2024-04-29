# ControlHorarios

## Descripción
El objetivo principal del proyecto es desarrollar una aplicación web que simplifique el registro y la asignación de horarios para empleados dentro de una empresa o institución. Esta herramienta se enfocará en proporcionar una interfaz dinámica y fácil de usar, utilizando el framework Angular junto con una librería de Gantt para gestionar eficientemente los horarios laborales.

**Características o Funcionalidades Clave:**
1. **Interfaz de Usuario Intuitiva:** Diseño y desarrollo de una interfaz de usuario amigable, tanto para administradores como para empleados, con componentes reutilizables y una estructura modular para una fácil comprensión y navegación.

2. **Gestión de Horarios:** Integración de una librería de Gantt para visualizar y gestionar los horarios de manera eficiente, permitiendo la creación, modificación y eliminación de turnos de trabajo, así como la capacidad de arrastrar y soltar para ajustar los horarios de manera intuitiva.

3. **Visualización de Carga de Trabajo:** Funcionalidad para visualizar la carga de trabajo de cada empleado, facilitando la distribución equitativa de las responsabilidades laborales.

4. **Detección de Conflictos de Horarios:** Implementación de características que detecten automáticamente conflictos de horarios, evitando superposiciones y asegurando una asignación adecuada de los turnos de trabajo.

5. **Autenticación y Autorización:** Medidas de seguridad para garantizar la autenticación y autorización de los usuarios, con diferentes niveles de acceso para administradores y empleados, asegurando la privacidad de los datos.

6. **Generación de Informes y Estadísticas:** Capacidad para generar informes y estadísticas sobre la distribución del tiempo laboral, facilitando el análisis y la toma de decisiones por parte de los administradores.

**Duración del Proyecto:**
El proyecto se desarrollará en varias etapas, con una duración estimada de seis meses desde la planificación inicial hasta la implementación y pruebas finales.

**Riesgos del Proyecto:**
Algunos posibles riesgos incluyen retrasos en el desarrollo debido a problemas técnicos inesperados, dificultades en la integración de la librería de Gantt, y desafíos en la implementación de medidas de seguridad robustas.

**Cronograma:**
1. Planificación y Diseño de la Interfaz de Usuario - 1 mes
2. Desarrollo de la Aplicación Angular - 2 meses
3. Integración de la Librería de Gantt - 1 mes
4. Implementación de Funcionalidades de Seguridad - 1 mes
5. Pruebas y Depuración - 1 mes

**Organigrama:**
El equipo estará compuesto por desarrolladores frontend y backend, un diseñador de interfaz de usuario, un especialista en seguridad de la información, y un coordinador de proyecto para supervisar y gestionar todas las etapas del desarrollo.
## Historias de Usuario 

### Empleado

- **HI-USA-001:** Como empleado, quiero poder solicitar mi horario para el próximo mes, eligiendo el tipo de turno que prefiero, para tener mayor flexibilidad y comodidad en mi jornada laboral.

  **Descripción:** Los empleados podrán solicitar su horario para el próximo mes a través de la aplicación, seleccionando el tipo de turno que prefieren.

  **Criterios de Aceptación:**
  - La aplicación permite a los empleados solicitar su horario para el próximo mes.
  - Los empleados pueden elegir el tipo de turno que prefieren.
  - La solicitud se realiza de manera clara y sencilla desde la interfaz de usuario.

- **HI-USA-002:** Como empleado, quiero ver mi horario mensual en un formato de Gantt para tener una visión clara y estructurada de mis turnos de trabajo, facilitando así la planificación de mis actividades fuera del trabajo.

  **Descripción:** Los empleados podrán visualizar su horario mensual en un formato de Gantt desde la aplicación.

  **Criterios de Aceptación:**
  - Los empleados pueden acceder a su horario mensual desde la aplicación.
  - El horario se muestra en un formato de Gantt claro y estructurado.
  - La visualización del horario facilita la planificación de actividades fuera del trabajo.

- **HI-USA-003:** Como empleado, quiero que la aplicación me indique claramente a qué sede pertenezco y a qué área de trabajo, para tener una referencia rápida de mi ubicación laboral.

  **Descripción:** Los empleados podrán ver claramente en la aplicación a qué sede y área de trabajo pertenecen.

  **Criterios de Aceptación:**
  - La aplicación muestra de forma clara la sede a la que pertenece el empleado.
  - La aplicación muestra de forma clara el área de trabajo del empleado.

- **HI-USA-004:** Como empleado, deseo tener la capacidad de solicitar vacaciones a través de la aplicación, indicando las fechas deseadas y asegurándome de que no haya conflictos con mi horario laboral, permitiéndome disfrutar de períodos de descanso sin afectar la operatividad del equipo.

  **Descripción:** Los empleados podrán solicitar vacaciones a través de la aplicación, indicando las fechas deseadas y evitando conflictos con su horario laboral.

  **Criterios de Aceptación:**
  - Los empleados pueden solicitar vacaciones desde la aplicación.
  - Los empleados pueden seleccionar las fechas deseadas para sus vacaciones.
  - La aplicación verifica que no haya conflictos con el horario laboral del empleado antes de aprobar la solicitud de vacaciones.

- **HI-USA-005:** Como empleado, quiero solicitar vacaciones visualizando los días disponibles, facilitando la elección de fechas que se ajusten tanto a mis necesidades como a la disponibilidad de la empresa.

  **Descripción:** Los empleados podrán solicitar vacaciones viendo los días disponibles en el calendario de la aplicación.

  **Criterios de Aceptación:**
  - La aplicación muestra de forma clara los días disponibles para solicitar vacaciones.
  - Los empleados pueden seleccionar las fechas de vacaciones basándose en los días disponibles en el calendario.

- **HI-USA-006:** Después de elegir mi turno deseado, la función de confirmación es rápida y eficiente, asegurando una respuesta inmediata para que pueda organizarme con anticipación.

  **Descripción:** Después de que los empleados elijan su turno deseado, la confirmación se realiza de manera rápida y eficiente.

  **Criterios de Aceptación:**
  - La aplicación proporciona una confirmación inmediata después de que el empleado elige su turno deseado.
  - La confirmación se realiza de manera eficiente, sin retrasos innecesarios.

- **HI-USA-007:** La aplicación me notifica vía correo electrónico sobre el veredicto de mi solicitud, que puede ser rechazado o aceptado, proporcionando una comunicación clara y oportuna sobre el estado de mi solicitud.

  **Descripción:** La aplicación envía notificaciones por correo electrónico a los empleados sobre el resultado de su solicitud de turno o vacaciones.

  **Criterios de Aceptación:**
  - La aplicación envía notificaciones por correo electrónico a los empleados sobre el resultado de su solicitud.
  - La notificación incluye si la solicitud fue aceptada o rechazada.
  - La comunicación es clara y oportuna, brindando al empleado información sobre el estado de su solicitud.

### Administrador

- **HI-USA-008:** Quiero gestionar y ajustar el número de empleados permitidos en cada tipo de turno, para garantizar una distribución equitativa de recursos y optimizar la asignación de tareas.

  **Descripción:** Los administradores podrán gestionar y ajustar el número de empleados permitidos en cada tipo de turno desde la aplicación.

  **Criterios de Aceptación:**
  - Los administradores pueden acceder a la configuración de cada tipo de turno desde la aplicación.
  - Los administradores pueden ajustar el número de empleados permitidos para cada tipo de turno.
  - Los cambios realizados se reflejan correctamente en la asignación de turnos.

- **HI-USA-009:** Deseo asignar periodos de training dentro del calendario de los empleados, para mejorar las habilidades y conocimientos del personal, contribuyendo al desarrollo profesional de manera planificada.

  **Descripción:** Los administradores podrán asignar periodos de training dentro del calendario de los empleados desde la aplicación.

  **Criterios de Aceptación:**
  - Los administradores pueden seleccionar los empleados a los que desean asignar periodos de training.
  - Los periodos de training se reflejan correctamente en el calendario de los empleados.
  - Los empleados reciben notificaciones sobre los periodos de training asignados.

- **HI-USA-010:** Deseo registrar a nuevos empleados en la aplicación y realizar cambios en sus horarios cuando sea necesario, para mantener actualizada la información del personal y adaptarla a las necesidades operativas.

  **Descripción:** Los administradores podrán registrar a nuevos empleados en la aplicación y realizar cambios en sus horarios cuando sea necesario.

  **Criterios de Aceptación:**
  - Los administradores pueden agregar nuevos empleados a la aplicación.
  - Los administradores pueden realizar cambios en los horarios de los empleados existentes según sea necesario.
  - La información del personal se mantiene actualizada y se adapta a las necesidades operativas.

- **HI-USA-011:** Deseo poder cargar información de forma masiva mediante archivos en formatos .xlsx,json y/o .csv, para facilitar la gestión eficiente de grandes cantidades de datos y mantener la consistencia en la base de información.

  **Descripción:** Los administradores podrán cargar información masiva mediante archivos en formatos .xlsx, .json y/o .csv para agilizar la gestión de grandes cantidades de datos y asegurar la consistencia en la base de información de la aplicación.

  **Criterios de Aceptación:**
  - La aplicación permite a los administradores cargar archivos en formatos .xlsx, .json y/o .csv desde la interfaz de usuario.
  - Los datos cargados se procesan correctamente y se reflejan en la base de información de la aplicación.
  - Se proporciona retroalimentación clara en caso de errores durante la carga de datos.

### Super Administrador

- **HI-USS-012:** El super administrador se loguea, visualiza y selecciona la lista de todos los administradores y la región que administran, para llevar un control centralizado de las funciones administrativas.

  **Descripción:** El super administrador podrá visualizar y seleccionar la lista de todos los administradores y las regiones que administran desde la aplicación para llevar un control centralizado de las funciones administrativas.

  **Criterios de Aceptación:**
  - El super administrador puede iniciar sesión en la aplicación con privilegios de super administrador.
  - La aplicación muestra una lista de todos los administradores registrados y las regiones que administran.
  - El super administrador puede seleccionar y acceder a la información detallada de cada administrador y región.

- **HI-USS-013:** Si selecciona a un administrador, visualiza todos los empleados que este administra, permitiendo un seguimiento detallado de la gestión de personal por parte de cada administrador.

  **Descripción:** Si el super administrador selecciona a un administrador específico, podrá visualizar todos los empleados que este administra desde la aplicación, permitiendo un seguimiento detallado de la gestión de personal por parte de cada administrador.

  **Criterios de Aceptación:**
  - El super administrador puede seleccionar a un administrador específico desde la interfaz de usuario.
  - La aplicación muestra una lista de todos los empleados que el administrador seleccionado administra.
  - El super administrador puede acceder a información detallada sobre la gestión de cada empleado por parte del administrador seleccionado.

- **HI-USS-014:** Quiero visualizar las jornadas de trabajo de cada empleado para determinar el mejor momento para sus vacaciones, facilitando la planificación y asegurando la continuidad operativa.

  **Descripción:** El super administrador podrá visualizar las jornadas de trabajo de cada empleado desde la aplicación para determinar el mejor momento para sus vacaciones y facilitar la planificación, asegurando la continuidad operativa.

  **Criterios de Aceptación:**
  - El super administrador puede acceder a la información de las jornadas de trabajo de cada empleado desde la interfaz de usuario.
  - La aplicación muestra de manera clara las jornadas de trabajo de cada empleado.
  - El super administrador puede utilizar esta información para planificar las vacaciones de los empleados y garantizar la continuidad operativa.

- **HI-USS-015:** Quiero dar de alta nuevos usuarios administradores y otros tipos de usuarios para tener más apoyo en la administración de las distintas regiones, garantizando una gestión eficiente y escalable.

  **Descripción:** El super administrador podrá dar de alta nuevos usuarios administradores y otros tipos de usuarios desde la aplicación para garantizar una gestión eficiente y escalable de las distintas regiones.

  **Criterios de Aceptación:**
  - El super administrador puede agregar nuevos usuarios administradores y otros tipos de usuarios desde la interfaz de usuario.
  - La aplicación verifica y valida los datos ingresados para el registro de nuevos usuarios.
  - Los nuevos usuarios registrados pueden acceder a la aplicación con los roles y permisos correspondientes.

- **HI-USS-016:** Quiero recibir alertas sobre posibles problemas de rendimiento o seguridad en la aplicación, para tomar medidas proactivas y mantener la estabilidad del sistema.

  **Descripción:** El super administrador recibirá alertas sobre posibles problemas de rendimiento o seguridad en la aplicación para tomar medidas proactivas y mantener la estabilidad del sistema.

  **Criterios de Aceptación:**
  - La aplicación monitorea de forma continua el rendimiento y la seguridad del sistema.
  - En caso de detectar problemas de rendimiento o seguridad, se envían alertas al super administrador.
  - Las alertas proporcionan información detallada sobre el problema detectado y posibles acciones a tomar.

- **HI-USS-017:** Necesito tener la capacidad de realizar copias de seguridad y restaurar datos en caso de pérdida o errores críticos, para asegurar la disponibilidad y la integridad de la información del sistema y garantizar la continuidad del servicio.

  **Descripción:** El super administrador tendrá la capacidad de realizar copias de seguridad y restaurar datos en caso de pérdida o errores críticos para garantizar la disponibilidad y la integridad de la información del sistema y garantizar la continuidad del servicio.

  **Criterios de Aceptación:**
  - La aplicación proporciona funciones para realizar copias de seguridad de la información del sistema.
  - La aplicación permite al super administrador restaurar datos a partir de las copias de seguridad en caso de pérdida o errores críticos.
  - Las operaciones de copia de seguridad y restauración de datos son rápidas, eficientes y seguras.
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
![Actividades](https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/07bc4e74-6ca6-4a67-881b-63d758849dd9)

### Diagrama de Clases
![DiClases](https://github.com/ABOK451/proyecto-control-horarios/assets/146273049/588de014-9b0b-4606-809b-a6f40cbd8315)

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
