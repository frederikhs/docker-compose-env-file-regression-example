# docker-compose-env-file-regression-example

This is a repository that illustrates the regression that happened to the `--env-file` command argument when Docker Compose updated from version [v2.27.0](https://github.com/docker/compose/releases/tag/v2.27.0) to [v2.27.1](https://github.com/docker/compose/releases/tag/v2.27.1).

In the [.github/workflows/test.yml](.github/workflows/test.yml) i have created a test to compare the result of running the `config` command with the `--env-file` argument to override the default `.env` file and use `.env.prod` instead.

The action **fails** on purpose because of the regression in [v2.27.1](https://github.com/docker/compose/releases/tag/v2.27.1)
