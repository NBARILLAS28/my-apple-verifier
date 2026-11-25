# Notas de verificación de AirPods

Notas reunidas al construir el verificador. Los datos de fuentes externas pueden cambiar; revísalos antes de apoyarte en ellos.

## Identificar el modelo

Apple imprime el número de modelo bajo cada AirPod, empezando con la letra A.

| Modelo | AirPod izquierdo | AirPod derecho | Estuche |
|---|---|---|---|
| AirPods Pro (2.ª gen., Lightning) | A2699 | A2698 | A2700 |
| AirPods Pro (2.ª gen., USB-C) | A3048 | A3047 | A2968 |
| AirPods Pro (1.ª gen.) | A2084 | A2083 | A2190 |

Fuente: [Identifica tus AirPods (Apple)](https://support.apple.com/en-ke/109525).

## Firmware

- Apple no ofrece una forma de instalar el firmware manualmente. Se entrega solo, mientras los AirPods se cargan y están al alcance Bluetooth de un iPhone, iPad o Mac.
- La versión 5E135 salió en mayo de 2023 para AirPods Pro 2 y otros modelos ([MacRumors](https://macrumors.com/2023/05/02/airpods-firmware-update-5e135)).
- En junio de 2026 ya circulaba una versión más reciente para AirPods Pro 2, la 8B41 ([gori.me](https://gori.me/?p=147571)).
- Dónde verla: Ajustes → Bluetooth → ⓘ junto a los AirPods → Versión.
- Conclusión práctica: unos originales conectados a un iPhone con iOS al día no deberían quedarse años en una versión de 2023. Una réplica no puede recibir firmware de Apple.

## Pruebas que aportan evidencia

| Prueba | Peso | Nota |
|---|---|---|
| Color blanco en estuche, AirPods y almohadillas | Alto | Apple vende los AirPods Pro solo en blanco, que sepamos. |
| Serial de Ajustes igual al impreso | Alto | Debe coincidir con la tapa del estuche y la base del AirPod. |
| Apple reconoce el serial en checkcoverage.apple.com | Alto | No es definitivo: las réplicas pueden copiar seriales reales. |
| El estuche suena desde la app Buscar | Alto | El estuche de los AirPods Pro 2 tiene altavoz propio. |
| Modelo impreso A2698 / A2699 | Medio | |
| Firmware reciente | Medio | Ver sección anterior. |
| Buscar con precisión del estuche | Medio | Requiere iPhone 11 o posterior. |
| Deslizar el tallo cambia el volumen | Medio | |
| Vendedor autorizado y precio parecido al de Apple | Medio | |
| Cancelación de ruido, prueba de almohadillas, caja sellada | Bajo | Subjetivas o fáciles de copiar. |

## Pruebas que no sirven

Las réplicas copian estas cosas, así que no cuentan a favor ni en contra:

- La animación de emparejamiento al abrir la tapa.
- El nombre «AirPods Pro», el porcentaje de batería y el menú de Audio espacial.
- El modelo y el serial que muestra Ajustes: iOS arma esa pantalla con lo que los audífonos dicen ser.
- La fila de cobertura en Ajustes: puede mostrar un serial real copiado.

## Si resultan falsos

- Pedir devolución por producto falsificado al vendedor o a la plataforma.
- Si se pagó con tarjeta, iniciar una disputa con el banco. Los plazos suelen ser cortos.
- Confirmar con un distribuidor autorizado de Apple o en [getsupport.apple.com](https://getsupport.apple.com).
