# Flutter Test `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for running Flutter unit tests

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/dluksza/flutter-test-pre-commit
  rev: "master"
  hooks:
    - id: flutter-test
```

## Testing nested Flutter project

By default `flutter test` is run in repository root, this should work for most of the cases.
When your Flutter project is nested somewhere in git repository or you have multiple modules
add `args` parameter to the hook configuration containing list of paths to the Flutter
projects, eg.:


```yaml
  hooks:
    - id: flutter-test
      args: [ module1, module2 ]
```


## Acknowledgements

[Charles Crete](https://github.com/Cretezy/) for creating `flutter-format-pre-commit`
