# pixel_perfect

[![Pub](https://img.shields.io/pub/v/pixel_perfect.svg)](https://pub.dartlang.org/packages/pixel_perfect)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/kherel/pixel_perfect)

Add semi transparent image to your screen.

![demo1](demo1.gif)
![demo2](demo2.gif)

## Getting started

Add pixel_perfect in your `pubspec.yaml` dependencies.

```yaml
dependencies:
 pixel_perfect: any
```

### How To Use

**Simple use**

Add assets folder with images to your `pubspec.yaml`

```yaml
  uses-material-design: true
  assets:
    - assets/
```

Import the following package in your dart file

```dart
import 'package:pixel_perfect/pixel_perfect.dart';
```

```dart

return PixelPerfect(
  assetPath: 'assets/design.png', // path to your asset image
  child: Scaffold(
    ..
  )
)
```

**Extended use**

```dart

return PixelPerfect.extended(
  image: Image.asset( // any image file
    'assets/element.png',
    scale: 2,
  ), 
  initBottom: 20, //  default bottom distance (optional)
  offset: Offset.zero, // default image offset (optional)
  child: Scaffold(
    ..
  )
)
```