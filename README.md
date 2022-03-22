[![Github Actions](https://github.com/vivitainc/flutter_collection_copy_extensions/actions/workflows/flutter-package-test.yaml/badge.svg)](https://github.com/vivitainc/flutter_collection_copy_extensions/actions/workflows/flutter-package-test.yaml)

## Features

List/Map/SetのCopy操作Extensionを提供する.

これらのExtensionはRedux Architectureで頻発する処理を書きやすくするために使用できる.

## Usage

```dart

final map = <String, String>{
    'Key1': 'Value1',
    'Key2': 'Value2',
};

final value2Copy = map.copyWhere((entry) => entry.value == 'Value2');
final removedKey1Copy = map.copyWhere((entry) => entry.key != 'Key1');

```
