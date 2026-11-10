# Ejemplo práctico: Estructura condicional if/else (Miniespecificación y Python)

- **Descripción:** Las estructuras condicionales permiten evaluar una condición lógica (Verdadero o Falso) para bifurcar el flujo de ejecución de un programa. A continuación, se presenta la representación mediante miniespecificación (pseudocódigo) y su equivalente directo en un script estructurado de Python.

- **Miniespecificación (Pseudocódigo):**

    ```text
    Inicio
        Leer edad
        Si edad >= 18 Entonces
            Imprimir "Es mayor de edad"
        Sino
            Imprimir "Es menor de edad"
        FinSi
    Fin
    ```

- **Ejemplo detallado en Python:**

    ```python
    # Ejemplo de estructura condicional if/else en Python
    if __name__ == "__main__":
        try:
            edad = int(input("Ingrese su edad: "))
            
            if edad >= 18:
                print("Es mayor de edad.")
            else:
                print("Es menor de edad.")
        except ValueError:
            print("Error: Debe ingresar un valor numérico entero válido.")
    ```

---
*Hecho por Miguel Camilo Téllez Jara para los compañeros de primer ciclo de la carrera de Ingeniería en Redes y Análisis de Datos, y para el Docente Tutor Mgtr. René Rolando Elizalde Solano. Materia: Fundamentos de Programación, 2026, UTPL.*