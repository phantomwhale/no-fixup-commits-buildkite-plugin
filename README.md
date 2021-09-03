# No Fixup Commits Buildkite Plugin

An [Buildkite plugin](https://buildkite.com/docs/agent/v3/plugins) for detecting if there are any `fixup` commits on the branch

It contains a [command hook](hooks/command), and [tests](tests/command.bats) using [plugin-tester](https://github.com/buildkite-plugins/plugin-tester).

## Example

```yml
steps:
  - plugins:
      - no-fixup-commits#v1.0.0: ~
```

## Tests

To run the tests of this plugin, run
```sh
docker-compose run --rm tests
```

## License

MIT (see [LICENSE](LICENSE))
