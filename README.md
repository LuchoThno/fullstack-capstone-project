Historia de Usuario 1 – Registro de Usuario

As a nuevo usuario
I need registrarme en la plataforma GiftLink
So that pueda acceder a la comunidad y compartir regalos

Details and Assumptions

El usuario debe ingresar nombre, correo electrónico y contraseña.

El correo electrónico debe ser único.

La contraseña debe almacenarse de forma segura usando hash.

El sistema debe validar que los campos obligatorios estén completos.

Acceptance Criteria
Given un usuario está en la página de registro
When ingresa nombre, correo electrónico y contraseña válidos
Then el sistema crea una nueva cuenta de usuario
And muestra un mensaje de registro exitoso
Historia de Usuario 2 – Inicio de Sesión

As a usuario registrado
I need iniciar sesión en la plataforma
So that pueda acceder a mi cuenta y gestionar mis regalos

Details and Assumptions

El usuario debe ingresar correo electrónico y contraseña.

El sistema valida las credenciales contra la base de datos.

Si las credenciales son correctas, el sistema inicia sesión.

Acceptance Criteria
Given el usuario está en la página de inicio de sesión
When ingresa su correo y contraseña correctos
Then el sistema autentica al usuario
And lo redirige al panel principal
Historia de Usuario 3 – Crear Publicación de Regalo

As a usuario registrado
I need publicar un regalo disponible
So that otros usuarios puedan verlo y solicitarlo

Details and Assumptions

El usuario debe ingresar título y descripción del regalo.

El usuario debe estar autenticado.

La publicación se guarda en la base de datos.

La publicación debe mostrarse en el feed de regalos.

Acceptance Criteria
Given el usuario está autenticado en la plataforma
When crea una publicación con título y descripción
Then el sistema guarda la publicación
And la muestra en la lista de regalos disponibles
Historia de Usuario 4 – Ver Regalos Disponibles

As a usuario de GiftLink
I need ver la lista de regalos disponibles
So that pueda encontrar regalos que me interesen

Details and Assumptions

El sistema debe obtener los regalos desde el backend.

Cada regalo debe mostrar título, descripción y usuario que lo publicó.

Acceptance Criteria
Given el usuario accede a la página principal
When el sistema carga las publicaciones de regalos
Then se muestra una lista de regalos disponibles
And cada regalo muestra su información básica
Historia de Usuario 5 – Solicitar un Regalo

As a usuario interesado
I need solicitar un regalo publicado
So that pueda recibirlo del usuario que lo ofrece

Details and Assumptions

Solo usuarios autenticados pueden solicitar regalos.

El sistema registra la solicitud en la base de datos.

El propietario del regalo debe poder ver las solicitudes.

Acceptance Criteria
Given el usuario está autenticado
And está viendo un regalo disponible
When presiona el botón "Solicitar"
Then el sistema registra la solicitud del regalo
And muestra un mensaje de confirmación
