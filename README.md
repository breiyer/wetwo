# Se divide en 3 Apps (roles)
---

### **App Estudiantes**
> - Registro - Login.
> - Configuración de cuenta.
> - Cambio de contraseña.
> - Olvidé mi contraseña.
> - Inscribirse en un curso.
> - Ver cursos inscritos.
> - Entrar a un curso inscrito.
> - Inscribirse en un examen.
> - Ver historial de exámenes.
> - Ver resultados de un examen completado.


&nbsp;

### **App Docentes**
> - Registro - Login.
> - Configuración de cuenta.
> - Cambio de contraseña.
> - Olvidé mi contraseña.
> - Crear curso.
> - Ver cursos creados.
> - Editar un curso creado.
> - Lanzar un curso creado.
> - Crear examen.
> - Ver exámenes creados.
> - Lanzar un examen creado.
> - Ver resultados de los exámenes lanzados.


&nbsp;

### **App Admin**
> - Ver estudiantes y docentes registrados.
> - Deshabilitar estudiantes y docentes registrados.
> - Eliminar estudiantes y docentes registrados.




&nbsp;

# Requerimientos
---

### **Registro y configuración de cuentas (docentes y estudiantes)**
> - El formulario para el registro de usuarios tendrá:
>   - Nombres.
>   - Apellidos.
>   - Documento de identidad (sea CC o tarjeta).
>   - Correo.
>   - Contraseña y repetir contraseña.
> - Para iniciar sesión se entra con correo y contraseña.
> - Se podrán cambiar todos los campos del usuario en la configuración.
> - Para recuperar la cuenta (olvidé contraseña) se envía un mensaje al 
>   correo de la cuenta con un link mediante el cual se resetea.


&nbsp;

### **Funcionalidades del rol estudiante**
>   &nbsp;
> 
>   - ##### Inscribir curso 
>     El estudiante ingresa el código del curso, como cuando 
>     un estudiante se inscribe en una materia en classroom. Luego, el 
>     curso les aparecerá en la lista de la sección [Cursos inscritos](#cursos-inscritos).
>   - ##### Cursos inscritos 
>     Lista con todos los cursos a los cuales se encuentra inscrito el estudiante. Al presionar 
>     click en uno de los cursos, redirige a la [sección donde el estudiante hace el curso](#sección-donde-el-estudiante-hace-el-curso).
>   - ##### Sección donde el estudiante hace el curso 
>     Los cursos se conforman por capítulos, estos a su vez, se conforman por; un título, 
>     una descripción, y un vídeo tutorial. Por lo anterior, ésta sección será una lista 
>     con todos los capítulos del curso. Al presionar click en un capítulo, se abrirá en 
>     una nueva ventana o en la existente el vídeo tutorial del capítulo.
> 
>   &nbsp;
> 
>   - ##### Inscribir un examen 
>     El estudiante ingresa el código del examen, luego, se abrirá en una nueva ventana o en la 
>     existente la [sección en donde el estudiante hace el examen](#sección-en-donde-el-estudiante-hace-el-examen), 
>     es decir, inmediatamente el estudiante ingresa el código del examen, el examen empieza.
>   - ##### Sección en donde el estudiante hace el examen
>     El examen tendrá un límite de tiempo desde que el estudiante lo inicia, asimismo, será de selección 
>     múltiple única respuesta. Adicional, las preguntas tendrán un orden aleatorio si así lo especifica 
>     el docente y, de la misma forma, las preguntas tendrán un vídeo o imagen de ayuda opcionalmente.
>   - ##### Historial de exámenes
>     Lista con todos los exámenes que el estudiante ha realizado. Al presionar click en uno de los 
>     exámenes, redirige a la [sección donde el estudiante ve el resultado del examen](#sección-donde-el-estudiante-ve-el-resultado-del-examen).
>   - ##### Sección donde el estudiante ve el resultado del examen
>     El estudiante podrá ver el tiempo que tardó realizando el examen, cuántas preguntas se hicieron, 
>     cuántas preguntas respondió, cuántas respondió bien, cuántas preguntas respondió mal, 
>     el nombre del examen, el profesor, y la fecha en que hizo el examen.


&nbsp;

### **Funcionalidades del rol docente**
>   &nbsp;
> 
>   - ##### Crear curso
>     El docente ingresa el nombre que tendrá el curso, a continuación, será redirigido a la 
>     [sección donde el docente administra el curso](#sección-donde-el-docente-administra-el-curso).
>   - ##### Sección donde el docente administra el curso
>     El docente podrá; crear, editar, ver y eliminar los capítulos que tendrá el curso, ver los 
>     estudiantes que se unieron al curso y, cambiar el nombre del curso. 
>     Asimismo, podrá lanzar el curso en el momento que desee. También, tendrá disponible en 
>     todo momento el código del curso para que los estudiantes puedan unirse, siempre y cuando 
>     el curso haya sido lanzado con anterioridad. De igual forma que lo anterior, tendrá 
>     visible la última fecha en que lanzó el curso.
>   - ##### Crear capítulo
>     El docente ingresa el nombre, la descripción y el vídeo tutorial del capítulo.
>   - ##### Lanzar curso
>     Lanzar el curso significa que éste será publicado para que los estudiantes se 
>     puedan unir, en caso de que el curso ya haya sido lanzado, lanzarlo nuevamente significa que 
>     está actualizando el contenido del curso publicado (lanzado anteriormente).
> 
>   &nbsp;
> 
>   - ##### Crear examen
>     El docente ingresa el nombre que tendrá el examen, a continuación, será redirigido a 
>     la [sección donde el docente administra el examen](#sección-donde-el-docente-administra-el-examen).
>   - ##### Sección donde el docente administra el examen
>     El docente podrá; crear, ver y eliminar las preguntas que tendrá el examen y, cambiar el 
>     nombre del examen. Asimismo, podrá lanzar el examen en el momento que desee.
>   - ##### Crear pregunta
>     Una vez el docente pulse el botón para añadir pregunta, se despliega una ventana 
>     emergente donde se le solicita; el enunciado de la pregunta, vídeo o imagen de 
>     ayuda (opcionalmente), las 4 posibles respuesta y, cuál de las 4 es la correcta.
>   - ##### Lanzar examen
>     Lanzar el examen significa que éste será publicado para que los estudiantes 
>     puedan ingresar a realizarlo, a diferencia de la funcionalidad de [lanzar curso](#lanzar-curso), 
>     los exámenes no pueden editados una vez que fueron lanzados, pues puede afectar a aquellos que 
>     lo estén realizando, por lo tanto, si se quiere modificar un examen, se deberá crear uno 
>     diferente y corregir allí dicho examen. Al lanzar el examen, se le solicita al docente que 
>     indique el tiempo máximo de duración que tendrá el examen, una vez lanzado el examen, se le 
>     mostrará al docente el código que tendrá el examen para que los estudiantes lo realicen.
>   - ##### Ver exámenes lanzados
>     El docente podrá ver una lista con los exámenes que ha lanzado, donde se destaca; la fecha en 
>     que fue lanzado, el nombre del examen, y la cantidad de participantes. Al presionar click 
>     sobre uno de los exámenes, lo redirige a la sección de [ver examen lanzado](#ver-examen-lanzado).
>   - ##### Ver examen lanzado
>     El docente podrá ver una lista con todos los estudiante que realizaron 
>     el examen, al presionar click sobre uno de los estudiantes, lo llevará a la sección de 
>     [ver resultado individual del examen](#ver-resultado-individual-del-examen).
>   - ##### Ver resultado individual del examen
>     El docente podrá ver todas las preguntas del examen, de cada pregunta podrá ver; el enunciado, 
>     las 4 posibles respuesta, la que era correcta, y la que el estudiante respondió. Asimismo, 
>     podrá ver; los nombres y apellidos, el documento de identidad, y el correo del estudiante 
>     responsable del resultado individual. También, podrá ver la cantidad de preguntas que tuvo 
>     el examen y, cuántas preguntas respondió bien y cuántas preguntas respondió mal el estudiante.

