# my-apple-verifier

Verificador de AirPods falsos. Una página web de una sola hoja (`index.html`) con una lista de pruebas guiadas para reunir evidencia sobre si unos AirPods Pro de 2.ª generación (A2698 / A2699, estuche A2700) son originales de Apple.

No certifica nada: ninguna prueba sola confirma si son falsos, y la verificación definitiva es con Apple.

## Qué hace

- 13 pruebas en cuatro grupos: a simple vista, Ajustes y Apple, funciones de los originales, y la compra.
- Cada prueba se responde con Sí, No o No sé, y trae una explicación de cómo probarla.
- Las señales de alerta suman un puntaje con peso alto, medio o bajo, y el resultado se actualiza en vivo.
- Genera un resumen que se puede copiar para enviarlo a un vendedor o al banco.
- Guarda las respuestas en el navegador (`localStorage`), sin enviar nada a ningún servidor.

## Cómo usarla

Abre `index.html` en el navegador del iPhone o publícala como sitio estático (Netlify, GitHub Pages). No tiene dependencias, salvo las fuentes de Google Fonts.

## Documentación

- [`docs/notas-verificacion.md`](docs/notas-verificacion.md): modelos, firmware, pruebas que sirven y pruebas que no, con fuentes.
- [`docs/fase-2-corebluetooth.md`](docs/fase-2-corebluetooth.md): plan y límites de una app nativa en iOS con CoreBluetooth.

## Fuera de alcance

Esta herramienta no actualiza ni modifica el firmware de ningún audífono. Apple firma y entrega el firmware de los AirPods por un canal privado, y una réplica no puede recibirlo.
