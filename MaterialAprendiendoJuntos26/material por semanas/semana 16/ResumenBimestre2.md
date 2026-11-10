# 4.8. Resumen y Consolidación del Segundo Bimestre (Semanas 9 a 15)

- **Descripción general:** Síntesis y estructuración de los contenidos avanzados del segundo bimestre de la materia, abarcando la gestión de excepciones, la persistencia de datos en archivos, el uso de librerías externas y los fundamentos de la Programación Orientada a Objetos (POO).

- **Estructura temática por semanas:**
  - **Semana 9 (Manejo de Excepciones y Control de Errores):** Estudio de errores en tiempo de ejecución, uso de bloques `try`, `except`, `else` y `finally`, y activación de excepciones personalizadas mediante `raise`.
  - **Semana 10 (Persistencia de Datos y Archivos de Texto):** Comprensión de la memoria volátil (RAM) frente al almacenamiento secundario, modos de apertura (`'r'`, `'w'`, `'a'`) y gestión eficiente con la sentencia `with`.
  - **Semana 11 (Técnicas Avanzadas de Lectura de Archivos):** Aplicación práctica de métodos integrados (`read()`, `readline()`, `readlines()`) e iteración optimizada línea por línea con bucles `for`.
  - **Semana 12 (Gestión de Librerías Externas):** Diferenciación entre bibliotecas estándar y paquetes externos, instalación mediante el gestor `pip`, e integración de herramientas como `requests`.
  - **Semana 13 (Introducción a la Programación Orientada a Objetos):** Transición hacia el paradigma de objetos, definición de clases, instanciación de objetos, atributos y métodos constructores (`__init__`).
  - **Semana 14 (Pilares y Propiedades de la POO):** Mecanismos de encapsulamiento, protección del estado interno y modelado de relaciones estructurales (asociación y agregación) mediante diagramas UML.
  - **Semana 15 (Integración y Proyecto Final):** Consolidación de flujos de trabajo en Python, manejo robusto de errores, persistencia modular y resolución de casos prácticos integrales.

- **Ejemplo integrado en Python (Clase orientada a objetos con persistencia y manejo de excepciones):**

    ```python
    class RegistroAcademico:
        def __init__(self, archivo_salida):
            self.archivo_salida = archivo_salida

        def registrar_nota(self, estudiante, nota):
            try:
                if nota < 0 or nota > 10:
                    raise ValueError("Error: La calificación debe estar en el rango de 0 a 10.")
                with open(self.archivo_salida, "a", encoding="utf-8") as f:
                    f.write(f"Estudiante: {estudiante} | Nota: {nota}\n")
                print(f"Registro guardado exitosamente para {estudiante}.")
            except ValueError as ve:
                print(ve)
            except Exception as e:
                print(f"Error inesperado al procesar el archivo: {e}")

    if __name__ == "__main__":
        sistema = RegistroAcademico("calificaciones_utpl.txt")
        sistema.registrar_nota("Miguel Téllez", 9.7)
    ```

---
*Hecho por Miguel Camilo Téllez Jara para los compañeros de primer ciclo de la carrera de Ingeniería en Redes y Análisis de Datos, y para el Docente Tutor Mgtr. René Rolando Elizalde Solano. Materia: Fundamentos de Programación, 2026, UTPL.*