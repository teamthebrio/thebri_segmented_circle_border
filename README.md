<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->

# TheBrio Segmented Circle Border!!
A package for creating segmented circle borders in flutter.

## Getting started
Add the package to your ```pubspec.yaml```:

```thebrio_segmented_circle_border: 0.0.1```

## Usage

Add it as a border:
```dart
import 'dart:math';

import 'package:flutter/material.dart';
import 'package:thebrio_segmented_circle_border/thebrio_segmented_circle_border.dart';

void main() => runApp(SegmentedCircleBorderExample());

class TheBrioSegmentedCircleBorderExample extends StatelessWidget {
  @override
  Widget build(BuildContext context) => Material(
      shape: TheBrioSegmentedCircleBorder(
          offset: -(112.5 * pi / 180),
          numberOfSegments: 8,
          sides: <BorderSide>[
            BorderSide(color: Color(0xFFFF0000), width: 10.0),
            BorderSide(color: Color(0xFF00FF00), width: 1.0),
            BorderSide(color: Color(0xFF0000FF), width: 2.0),
            BorderSide(color: Color(0xFFFF0000), width: 3.0),
            BorderSide(color: Color(0xFF00FF00), width: 4.0),
            BorderSide(color: Color(0xFF0000FF), width: 5.0),
            BorderSide(color: Color(0xFFFF00000), width: 6.0),
            BorderSide(color: Color(0xFF00FF00), width: 7.0),
          ]),
      child: Container(
        width: 100,
        height: 100,
      ));
}
```