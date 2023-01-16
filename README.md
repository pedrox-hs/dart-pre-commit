# Dart pre-commit hooks

Some Dart hooks for [pre-commit](https://github.com/pre-commit/pre-commit).

Can be used in Flutter projects.

### Using dart-pre-commit with pre-commit

Add this to your `.pre-commit-config.yaml`

```yaml
- repo: https://github.com/pedrox-hs/flutter-pre-commit
  rev: v1.1.0  # Use the ref you want to point at
  hooks:
  - id: dart-analyze
  # - id: ...
```

### Hooks available

#### `dart-analyze`
Analyze Dart code.

#### `dart-format`
Dart source code format.

By default it just check for code format, to apply format use:

```yaml
  - id: dart-format
    args: ["--output=write"]
```

#### `dart-fix`
Apply automated fixes to Dart source code.

#### `fvm-dart-analyze`
Alternative for [`dart-analyze`](#dart-analyze) with FVM.

#### `fvm-dart-format`
Alternative for [`dart-format`](#dart-format) with FVM.

#### `fvm-dart-fix`
Alternative for [`dart-fix`](#dart-fix) with FVM.
