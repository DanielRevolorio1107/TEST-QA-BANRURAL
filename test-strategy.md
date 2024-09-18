# Errores Encontrados y Soluciones

## 1. Error en la Generación del Número Aleatorio
- **Descripción del Error:** El número aleatorio se generaba incorrectamente utilizando `Math.random() * 10`, lo que limitaba el rango entre 0 y 10.
- **Solución:** Cambié la lógica para que fuera `Math.floor(Math.random() * 100) + 1`, asegurando que el número estuviera entre 1 y 100.

## 2. Validación de Entrada Inadecuada
- **Descripción del Error:** El código no validaba si la entrada del usuario era un número entero, lo que podía llevar a errores al comparar.
- **Solución:** Implementé una validación que verifica si la entrada es un número entero y está dentro del rango de 1 a 100. Si no lo es, muestra una alerta y no se incrementa el contador de intentos.

## 3. Problema con el Manejo de Eventos
- **Descripción del Error:** Se usó `addeventListener` en lugar de `addEventListener`, lo que causaba que el evento no se registrara.
- **Solución:** Corregí el nombre del método a `addEventListener` para asegurar que los eventos se manejen correctamente.

## 4. Mensajes de Resultado Incorrectos
- **Descripción del Error:** Los mensajes mostrados al usuario no reflejaban correctamente el estado del juego (por ejemplo, los mensajes de victoria y derrota estaban invertidos).
- **Solución:** Reorganicé la lógica de mensajes en la función `checkGuess`, asegurando que el mensaje correcto se muestre en cada caso.

## 5. Error en la Re-inicialización del Juego
- **Descripción del Error:** Al reiniciar el juego, el número aleatorio no se regeneraba correctamente.
- **Solución:** Actualicé la lógica en la función `resetGame` para regenerar un nuevo número aleatorio correctamente al inicio de un nuevo juego.

## 6. Problema en la Visualización de Resultados
- **Descripción del Error:** No se estaban aplicando correctamente las clases CSS para los mensajes de resultado.
- **Solución:** Añadí clases a los elementos `lastResult` y `lowOrHi` para aplicar el estilo correspondiente según el resultado del juego.

## 7. No Se Limpiaba el Campo de Entrada
- **Descripción del Error:** El campo de entrada no se limpiaba adecuadamente después de cada intento.
- **Solución:** Implementé `guessField.value = ''` después de cada intento para asegurarse de que el campo se limpie.

## 8. Errores en la Consola del Navegador
- **Descripción del Error:** Se encontraron varios errores en la consola relacionados con la lógica de eventos y validaciones.
- **Solución:** Se revisaron los mensajes de la consola y se realizaron las correcciones necesarias según las recomendaciones del líder del equipo.

## 9. Cierre de etiqueta Body
-**Descripción del Error:** Se encontró el cierre de la etiqueta body en un lugar incorrecto.
-**Solución:** Se colocó la etiqueta en el lugar correcto para que todo el codigo este dentro de la misma.
