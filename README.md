# Roboregos-team

1. Descripción del Proyecto

Este proyecto es un robot autónomo desarrollado para la competencia "Candidates 2024" del equipo RoBorregos. El robot debe completar una serie de desafíos en tres pistas diferentes (Pista A, B y C), además de cruzar una rampa tipo sube y baja. Cada pista implica distintos sensores y lógicas de programación para seguir líneas, detectar colores, evitar obstáculos y completar objetivos específicos.

2. Requisitos del Sistema
Hardware Utilizado

    Arduino Uno (o similar)
    Motores DC con encoders
    Encoders rotativos para redundancia en control de movimiento
    Sensor ultrasónico (para detección de distancias y obstáculos)
    Sensor de color (para detección de colores específicos en Pista A y C)
    Sensor de línea infrarrojo (para seguimiento de línea en Pista B)
    Giroscopio de 3 ejes (para estabilización en el sube y baja)
    Gripper o mecanismo de agarre (para la pelota en Pista A)


   Software Utilizado/ Librerias

    Arduino IDE: Para cargar los códigos en el microcontrolador.
    Librerías Arduino:
        Encoder.h: Para manejar los encoders de los motores.
        Ultrasonic.h: Para controlar el sensor ultrasónico.
        Adafruit_TCS34725.h: Para el sensor de color.
        MPU6050.h: Para el giroscopio de 3 ejes.

   candidates2024-robot/
    │
    ├── TrackA.ino          # Código para la Pista A (Desafío de la Pelota)
    ├── TrackB.ino          # Código para la Pista B (Seguimiento de Línea)
    ├── TrackC.ino          # Código para la Pista C (Laberinto)
    ├── Seesaw.ino          # Código para el sube y baja
    ├── main.ino            # Código principal que coordina las pistas y el sube y baja

README - Competencia "Candidates 2024" - Proyecto de Robot Autónomo
1. Descripción del Proyecto

Este proyecto es un robot autónomo desarrollado para la competencia "Candidates 2024" del equipo RoBorregos. El robot debe completar una serie de desafíos en tres pistas diferentes (Pista A, B y C), además de cruzar una rampa tipo sube y baja. Cada pista implica distintos sensores y lógicas de programación para seguir líneas, detectar colores, evitar obstáculos y completar objetivos específicos.
2. Requisitos del Sistema
Hardware Utilizado

    Arduino Uno (o similar)
    Motores DC con encoders
    Encoders rotativos para redundancia en control de movimiento
    Sensor ultrasónico (para detección de distancias y obstáculos)
    Sensor de color (para detección de colores específicos en Pista A y C)
    Sensor de línea infrarrojo (para seguimiento de línea en Pista B)
    Giroscopio de 3 ejes (para estabilización en el sube y baja)
    Gripper o mecanismo de agarre (para la pelota en Pista A)

Software Utilizado

    Arduino IDE: Para cargar los códigos en el microcontrolador.
    Librerías Arduino:
        Encoder.h: Para manejar los encoders de los motores.
        Ultrasonic.h: Para controlar el sensor ultrasónico.
        Adafruit_TCS34725.h: Para el sensor de color.
        MPU6050.h: Para el giroscopio de 3 ejes.

3. Instrucciones de Instalación

    Clonar el Repositorio: Clona este repositorio en tu entorno local:

    bash

    git clone https://github.com/tu-usuario/candidates2024-robot.git

    Instalar las Librerías Necesarias: Asegúrate de tener instaladas todas las librerías mencionadas en los requisitos de software. Puedes instalarlas desde el gestor de librerías del Arduino IDE.
    Conectar Componentes: Conecta los motores, sensores y actuadores de acuerdo con el esquema de hardware proporcionado en la carpeta docs/.
    Subir el Código al Arduino: Carga los archivos .ino en el Arduino desde el Arduino IDE.

4. Estructura del Proyecto

Este repositorio está organizado de la siguiente manera:

plaintext

candidates2024-robot/
│
├── TrackA.ino          # Código para la Pista A (Desafío de la Pelota)
├── TrackB.ino          # Código para la Pista B (Seguimiento de Línea)
├── TrackC.ino          # Código para la Pista C (Laberinto)
├── Seesaw.ino          # Código para el sube y baja
├── main.ino            # Código principal que coordina las pistas y el sube y baja

Descripción de los Archivos Principales

    TrackA.ino: Contiene la lógica de control para detectar la pelota azul y llevarla al final de la pista.
    TrackB.ino: Controla los sensores infrarrojos para el seguimiento de la línea negra en la Pista B.
    TrackC.ino: Incluye la lógica para la detección de colores en el laberinto y la navegación autónoma.
    Seesaw.ino: Maneja la estabilidad y equilibrio del robot en la rampa del sube y baja.
    main.ino: Coordinador general que ejecuta las pistas en el orden correspondiente.

5. Contribuciones del Equipo

Cada miembro del equipo debe documentar su trabajo en este apartado, indicando qué cambios o implementaciones realizó en el proyecto.

[Daniel Alejandro Garcia Montiel A01253469]

    Tareas principales:
    Mecanica y construccion del robot.
    Sensor de lineas Seguidor.
    Cambios realizados:
    Crear repositorio lineamientos, leer el manual del reto y estipular lo que se debe hacer en cada parte.

[Nombre del Miembro 2]

    Tareas principales:
        Programación del seguimiento de línea en la Pista B.
        Optimización del tiempo de respuesta de los sensores infrarrojos.
    Cambios realizados:
        Reducción de la velocidad del motor en las curvas para evitar salirse de la línea.
        Corrección de errores en la detección de línea negra.

[Nombre del Miembro 3]

    Tareas principales:
        Programación de la navegación en el laberinto (Pista C).
        Implementación del sensor ultrasónico para evitar colisiones con paredes.
    Cambios realizados:
        Mejora en el algoritmo de detección de dead ends (casillas negras).
        Ajuste de los tiempos de giro con encoders para mejorar la precisión en los movimientos.

[Nombre del Miembro 4]

    Tareas principales:
        Implementación de la lógica de equilibrio para el sube y baja.
        Uso del giroscopio para controlar la inclinación en la rampa.
    Cambios realizados:
        Ajuste de la velocidad del robot en la rampa para evitar volcaduras.
        Mejoras en el manejo del equilibrio en el centro del sube y baja.

        6. Registro de Cambios

Mantén un historial de los cambios más importantes realizados en el proyecto.
Versión 1.0 - [19/10/2024]

    Configuración inicial del proyecto.
    Implementación de las pistas A, B, y C.
    Lineamientos y descripcion del reto division de labores.

Versión 1.1 - [Fecha]

    Optimización de los algoritmos de detección de color y seguimiento de línea.
    Mejora en la precisión de los encoders para el control de motores.
