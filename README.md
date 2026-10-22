# Agenda del IV Congreso de IA de Andalucía

Agenda interactiva de los días **27 y 28 de octubre de 2026** del IV Congreso de Inteligencia Artificial de Andalucía (Palacio de Congresos de Granada). Permite ver las sesiones por hora y sala, elegir a cuáles asistir y detectar cuándo dos coinciden.

> **Propuesta de rediseño no oficial.** Es un trabajo de clase. No pertenece a la organización del congreso ni a la Junta de Andalucía. El programa válido es siempre el [oficial](https://www.juntadeandalucia.es/congresoIA/programa/).

**Enlace:** [agenda-congreso-ia](https://agenda-congreso-ia.vercel.app/)

## Qué hace

- Muestra las sesiones del martes 27 y el miércoles 28 en una rejilla con una columna por sala (Manuel de Falla, Andalucía I, II y III).
- Cada sesión incluye hora de inicio y fin, duración, tipo (ponencia, mesa, taller, acto), ponentes y descripción cuando el programa la da.
- Al pulsar una sesión se añade a **Mi agenda**. Si dos sesiones elegidas se solapan, las marca en la rejilla y en la agenda.
- Las mesas tecnológicas se tratan aparte, porque son talleres de entrada libre que se repiten cada 30 minutos.
- Filtros por sala y la opción «Solo mi selección».
- Botón para copiar la agenda como texto.
- La selección se guarda en el navegador (`localStorage`). No hay servidor ni cuentas.
- Adaptada a móvil: por debajo de 760 px las columnas pasan a una lista por hora.

## Cómo está hecho

- Un único archivo `index.html` con HTML, CSS y JavaScript sin dependencias ni paso de compilación.
- Tipografía [Funnel Display](https://fonts.google.com/specimen/Funnel+Display) desde Google Fonts, la misma familia que usa la web del congreso para el texto.
- Estilo inspirado en la web del congreso: degradado de verde azulado a azul noche, barras de día, tarjetas de sesión y botones amarillos.
- Diseño siempre claro, para que el horario tenga fondo blanco en cualquier dispositivo.

## Cómo se hizo

Proyecto hecho con Claude, **orquestado por Miguel Ángel Herrera Serrano**, estudiante de primer año de Desarrollo de Aplicaciones Web. El trabajo se fue dirigiendo por conversación: objetivo, estilo visual, correcciones de fondo y de móvil, y publicación.

## Datos

Las sesiones se copiaron del [programa oficial](https://www.juntadeandalucia.es/congresoIA/programa/) el **20 de octubre de 2026**. Si la organización cambia algo después, esta página no se actualiza sola. Para corregir un dato, edita el bloque de sesiones dentro de `index.html`: cada línea `add(día, sala, 'hora', minutos, 'tipo', 'título', 'ponentes', 'descripción')` es una sesión.

El programa no publica sesiones para algunas franjas de ciertas salas (por ejemplo, la mañana del martes antes de las 12:00 en Andalucía I, II y III), y esta página lo refleja tal cual.

## Probarlo en local

Abre `index.html` en el navegador. No necesita nada más.

## Publicado con Vercel

Cada cambio que se suba a GitHub se publica solo.

https://agenda-congreso-ia.vercel.app/

