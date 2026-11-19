# Ronda 1. Preparar el proyecto
```
$ flutter create super_dolores
$ cd super_dolores
```
Esta app no usa paquetes externos: todo el dominio es Dart puro. Copia los archivos de lib/ y test/ siguiendo este manual.

```
📄 pubspec.yaml
name: super_dolores
description: SuperApp didáctica de Dolores Hidalgo - mensajería, pagos, comercio y transporte en un solo ecosistema.
publish_to: 'none'
version: 1.0.0+1

environment:
  sdk: ^3.4.0

# Esta app NO necesita paquetes externos: el dominio es Dart puro y los servicios son simulados.
dependencies:
  flutter:
    sdk: flutter

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^4.0.0

flutter:
  uses-material-design: true
```
Compruebe que todo corre: flutter test (fallará hasta que escribas el código, que es justo el punto del ciclo rojo-verde).

⚠️ Cuidado

Cambia el nombre del paquete en pubspec.yaml a super_dolores: las importaciones de las pruebas dependen de él (import "package:super_dolores/...").

