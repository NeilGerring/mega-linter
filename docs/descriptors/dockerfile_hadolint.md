<!-- markdownlint-disable MD033 MD041 -->
<!-- Generated by .automation/build.py, please do not update manually -->
# <a href="https://github.com/hadolint/hadolint" target="blank" title="Visit linter Web Site"><img src="https://hadolint.github.io/hadolint/img/cat_container.png" alt="hadolint" height="100px"></a>hadolint

- Web Site: [**https://github.com/hadolint/hadolint**](https://github.com/hadolint/hadolint#readme)
- Version: **1.18.2**

## Configuration

### hadolint configuration

- [Configure hadolint rules](https://github.com/hadolint/hadolint#configure)
  - If custom .hadolint.yml is not found, [.hadolint.yml](https://github.com/nvuillam/mega-linter/tree/master/TEMPLATES/.hadolint.yml) will be used
- [Disable hadolint rules in files](https://github.com/hadolint/hadolint#inline-ignores)

### Mega-linter configuration

- Enable hadolint by adding `DOCKERFILE_HADOLINT` in [ENABLE_LINTERS variable](https://github.com/nvuillam/mega-linter#activation-and-deactivation)
- Disable hadolint by adding `DOCKERFILE_HADOLINT` in [DISABLE_LINTERS variable](https://github.com/nvuillam/mega-linter#activation-and-deactivation)

| Variable | Description | Default value |
| ----------------- | -------------- | -------------- |
| DOCKERFILE_HADOLINT_ARGUMENTS | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"` |  |
| DOCKERFILE_HADOLINT_FILTER_REGEX_INCLUDE | Custom regex including filter<br/>Ex: `\/(src\|lib)\/` | Include every file |
| DOCKERFILE_HADOLINT_FILTER_REGEX_EXCLUDE | Custom regex excluding filter<br/>Ex: `\/(test\|examples)\/` | Exclude no file |
| DOCKERFILE_HADOLINT_FILE_NAME | hadolint configuration file name</br>Use `LINTER_DEFAULT` to let the linter find it | `.hadolint.yml` |
| DOCKERFILE_HADOLINT_RULES_PATH | Path where to find linter configuration file | Workspace folder, then Mega-Linter default rules |
| DOCKERFILE_HADOLINT_DISABLE_ERRORS | Run linter but disable crash if errors found | `false` |

## Behind the scenes

### How are identified applicable files

- File names:
  - `Dockerfile`


### Example calls

```shell
hadolint Dockerfile
```

```shell
hadolint -c .dockerfilelintrc Dockerfile
```


### Help content

```shell
hadolint - Dockerfile Linter written in Haskell

Usage: hadolint [-v|--version] [-c|--config FILENAME] [-f|--format ARG]
                [DOCKERFILE...] [--ignore RULECODE]
                [--trusted-registry REGISTRY (e.g. docker.io)]
  Lint Dockerfile for errors and best practices

Available options:
  -h,--help                Show this help text
  -v,--version             Show version
  -c,--config FILENAME     Path to the configuration file
  -f,--format ARG          The output format for the results [tty | json |
                           checkstyle | codeclimate | codacy] (default: tty)
  --ignore RULECODE        A rule to ignore. If present, the ignore list in the
                           config file is ignored
  --trusted-registry REGISTRY (e.g. docker.io)
                           A docker registry to allow to appear in FROM
                           instructions

```

### Installation on mega-linter Docker image

- Dockerfile commands :
```dockerfile
FROM hadolint/hadolint:latest-alpine as dockerfile-lint
COPY --from=dockerfile-lint /bin/hadolint /usr/bin/hadolint
```
