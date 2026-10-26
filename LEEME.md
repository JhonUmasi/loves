# Conecta — Un atlas de encuentros

Una aplicación personal en español para conocerte, practicar conversaciones y construir vínculos con reciprocidad. No necesita cuenta, instalaciones ni conexión a Internet.

## La nueva experiencia

El mapa es un paisaje ilustrado que puedes arrastrar con el ratón o recorrer con el dedo. Usa las flechas, el zoom o **Mi siguiente parada** para moverte. Cada estación abre su etapa. La vista **Índice** ofrece una alternativa de lectura sin desplazarse por el mapa.

Dentro de cada misión puedes marcar pasos individuales, desplegar un ejemplo y escribir una reflexión. Los pasos también se guardan y se incluyen en el respaldo. Completar una misión pone un sello de progreso y lanza una pequeña celebración visual (respeta la preferencia de movimiento reducido).

**Un reto sorpresa** elige una misión pendiente al azar. Tú decides si te apetece. **¿Con qué energía llegas hoy?** propone una acción según cómo te sientes en ese momento; esa elección temporal no modifica tu progreso. La pausa de respiración es opcional y tiene botones para empezar, detener y repetir.

En **Palabras**, abre las páginas desplegables para leer ejemplos y copiarlos. En **Ensaya**, elige una de las seis situaciones. El diario ahora se llama **Bitácora**, y **Mi mochila** abre el exportador e importador.

Los respaldos v1 anteriores siguen siendo compatibles. Si no contienen pasos individuales, se inician vacíos; las misiones ya completadas se muestran como practicadas.

## Abrir

Haz doble clic en `index.html`. Conserva `styles.css`, `data.js`, `app.js` y la carpeta `assets` junto al HTML.

También puedes servir la carpeta con Python:

```powershell
cd D:\Proyectos\Amor
python -m http.server 5173 --bind 127.0.0.1
```

Abre http://127.0.0.1:5173 en tu navegador. Para detener ese servidor, pulsa Ctrl+C en su terminal.

Usa siempre el mismo navegador y la misma forma de abrir la aplicación para ver el mismo guardado local. Un HTML abierto como archivo y una dirección HTTP tienen almacenamientos diferentes. Puedes trasladar el proceso entre ellos exportando e importando.

## Lo que incluye

- Ruta abierta de 8 etapas y 24 misiones, con ejercicios, ejemplos, notas y progreso.
- 6 simulaciones guiadas, con 18 decisiones y 54 opciones explicadas. Puedes repetirlas.
- 20 herramientas para conversar, invitar, poner límites y cuidar un vínculo, con búsqueda, categorías y copia de ejemplos.
- 12 ideas para citas, con filtros de ambiente, presupuesto y lugar, instrucciones e ideas guardadas.
- Plan de 30 días, con fecha de inicio configurable y actividades marcables.
- Diario con fecha, estado de ánimo, etapa, búsqueda, edición y eliminación.
- Perfil personal con intención y ritmo de práctica.
- Brújula sobre reciprocidad, autonomía, límites y consentimiento.
- Diseño adaptable a móvil, navegación por teclado y soporte de movimiento reducido.
- Guardado automático local y respaldo completo en JSON.

## Guardar y restaurar

1. Pulsa **Mi mochila** (el icono de descarga en móvil).
2. Elige **Descargar respaldo JSON**. Revisa la carpeta de descargas de tu navegador.
3. Conserva ese archivo en un lugar privado.
4. Para recuperarlo, pulsa **Elegir archivo JSON**.
5. Revisa el resumen y pulsa **Restaurar este proceso**. Puedes exportar el proceso actual antes de reemplazarlo.

El respaldo incluye perfil, misiones, notas, prácticas, plan, diario e ideas favoritas. El importador comprueba formato y versión antes de cambiar el proceso. Admite archivos de hasta 5 MB. Las notas y reflexiones se guardan como texto legible, sin cifrado. No compartas el respaldo si contiene información privada.

El navegador guarda el proceso al completar misiones, escribir notas, registrar días, terminar prácticas, guardar ideas, guardar una entrada del diario o guardar preferencias. Los formularios de diario y perfil requieren pulsar su botón **Guardar**. No hay sincronización en la nube. Borrar los datos del navegador o usar una ventana privada puede eliminar el guardado local; exporta copias periódicamente.

## Progreso

Los puntos reconocen tu práctica: 25 XP por misión, 5 por día del plan, 10 por escenario completado y 5 por reflexión (hasta 30 reflexiones). Repetir una actividad no duplica sus puntos. Desmarcar una actividad o eliminar una reflexión actualiza el total.

No hay bloqueos ni plazos obligatorios. Completar la ruta no garantiza una relación y no depende de convencer a otra persona. El contenido es orientación práctica, no terapia. El simulador usa guiones locales y no utiliza IA ni servicios externos.

## Archivos

- `index.html`: estructura y punto de entrada.
- `styles.css`: diseño, móvil e impresión.
- `data.js`: etapas, misiones, escenarios, herramientas, citas y plan.
- `app.js`: navegación, interacciones, guardado y respaldos.
- `assets/favicon.svg`: icono local.
- `assets/atlas-paisaje.png`: paisaje original generado para el mapa.
- `assets/GENERACION.md`: prompt y procedencia de la ilustración.

Puedes personalizar los textos en `data.js`. Conserva los identificadores de misiones y escenarios y el orden de las citas para mantener la compatibilidad de los respaldos existentes.
