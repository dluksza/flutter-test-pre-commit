# Flutter Test `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for running Flutter unit tests

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/dluksza/flutter-test-pre-commit
  rev: "master"
  hooks:
    - id: flutter-test
```

## Acknowledgements

[Charles Crete](https://github.com/Cretezy/) for creating `flutter-format-pre-commit`
