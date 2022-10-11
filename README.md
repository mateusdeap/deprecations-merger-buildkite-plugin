# Deprecations Merger Buildkite Plugin

This a buildkite plugin intended for use with the [next_rails](https://www.github.com/fastruby/next_rails) gem.

## Installation

Just add this to you `pipeline.yml`:

```yml
steps:
  - label: "Generate deprecations list"
  - plugins:
    - mateusdeap/deprecations-merger#v1.0.0
      pattern: '<name-pattern-of-your-deprecation-files>'
```

As an example, if you've configured `next_rails` to generate files named, `deprecations_shitlist0.json`, `deprecations_shitlist1.json` and so forth, than the `pattern` argument should be `'deprecations_shitlist*.json'`.

**WARNING:** This is still in a testing phase. It may not even work.
