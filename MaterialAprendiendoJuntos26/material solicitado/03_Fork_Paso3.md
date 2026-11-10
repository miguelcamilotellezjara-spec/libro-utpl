# Parte 3: Edición, registro y sincronización de cambios (Subir cambios)

- **Descripción:** Guía paso a paso para realizar modificaciones en el código fuente, preparar el seguimiento de archivos, confirmar los cambios localmente y sincronizarlos de forma segura con el repositorio remoto en GitHub mediante tokens de acceso personal.

- **Pasos a seguir para la sincronización:**
  - **Paso 8:** Revise los archivos del proyecto, realice la modificación solicitada en el código fuente, ejecute el programa para verificar su correcto funcionamiento y guarde los cambios.
  - **Paso 9:** Vuelva a abrir Git Bash, navegue hasta la carpeta del proyecto utilizando el comando `cd` seguido de la ruta de ubicación (`cd [ruta]`) y añada los archivos modificados escribiendo `git add .`.
  - **Paso 10:** Registre los cambios realizados escribiendo el mensaje de confirmación mediante el comando `git commit -m "Descripción de su cambio"`.
  - **Paso 11:** Diríjase nuevamente a Google Chrome, ingrese a los ajustes de desarrollador de su cuenta de GitHub y genere un token de acceso personal clásico (*Personal Access Token*).
  - **Paso 12:** Finalmente, regrese a Git Bash, ejecute el comando para enviar los cambios (`git push`) y, cuando el sistema lo solicite, pegue el token generado como contraseña para completar la sincronización exitosamente.

---
*Hecho por Miguel Camilo Téllez Jara para los compañeros de primer ciclo de la carrera de Ingeniería en Redes y Análisis de Datos, y para el Docente Tutor Mgtr. René Rolando Elizalde Solano. Materia: Fundamentos de Programación, 2026, UTPL.*