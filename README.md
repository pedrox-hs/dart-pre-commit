# Dart pre-commit hooks

Some Dart hooks for pre-commit.

Can be used in Flutter projects.

See also: https://github.com/pre-commit/pre-commit

### Using dart-pre-commit with pre-commit

Add this to your `.pre-commit-config.yaml`

```yaml
- repo: https://github.com/pedrox-hs/flutter-pre-commit
  rev: v1.0.0
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
