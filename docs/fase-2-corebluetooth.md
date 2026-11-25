# Fase 2: app nativa con CoreBluetooth

Estado: plan, sin implementar. Hay que validar la hipótesis principal en un iPhone real antes de construir nada más.

## Límites conocidos

- Los AirPods transmiten el audio por Bluetooth clásico y usan un canal privado de Apple. CoreBluetooth solo trabaja con Bluetooth de bajo consumo (BLE), así que, hasta donde se sabe, una app no puede leer el serial ni el firmware de unos AirPods emparejados.
- iOS puede ocultar parte de los datos de fabricante de los anuncios BLE de dispositivos de Apple. Esto hay que comprobarlo en un teléfono real.
- No se puede ni se debe flashear firmware: Apple lo firma y lo entrega por su cuenta, y una réplica no puede recibirlo.

## Hipótesis a validar

Los AirPods originales emiten un anuncio BLE con formato de Apple (identificador de fabricante `0x004C`) al abrir la tapa del estuche. Muchas réplicas no lo emiten, o lo emiten con otro formato. Si iOS expone esos datos, un escáner podría aportar una prueba más a la lista.

## Alcance propuesto

1. Escáner BLE con `CBCentralManager`: lista nombre, intensidad de señal (RSSI) y datos de fabricante de cada dispositivo cercano.
2. Decodificar el identificador de fabricante y mostrar si el anuncio parece de Apple.
3. Comparar el comportamiento con unos AirPods originales conocidos y con los AirPods bajo sospecha.
4. Si la hipótesis se confirma, integrar el resultado como una prueba más del verificador web o de una app propia.

## Requisitos

- Mac con Xcode y SwiftUI.
- Un iPhone real, porque el simulador no tiene Bluetooth.
- `NSBluetoothAlwaysUsageDescription` en `Info.plist`.
- Sin cuenta de desarrollador de pago, la app instalada en el propio iPhone caduca a los 7 días.
