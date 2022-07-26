# Introduction

This is demo application to show how to work with [Temporal](https://github.com/temporalio/sdk-php) from Symfony application.

This package based on [BaldinofRoadRunnerBundle](https://github.com/Baldinof/roadrunner-bundle).

Temporary used fork https://github.com/xepozz/roadrunner-bundle/tree/add-temporal-support before it will be merged into original repo.

## Installation
Install PHP dependencies:

```shell
composer i --prefer-dist
```

Get RoadRunner binary:

```shell
./vendor/bin/rr get-binary
```

Run docker containers:

```shell
docker-compose up -d
```

Run RoadRunner with debug mode (`-d` flag):

```shell
./rr serve -d
```

## Usage

Now you can open [http://localhost:8080](http://localhost:8080/)
and see small description about examples:

```
This project is example how to use Temporal with Symfony application.
There are exist several examples how it works.
Examples:
If you want to see how "simple" workflow works click here.
There is usual call non-blocking action. It should work as faster as you can run usual php code.
If you want to see how "complicated" workflow works click here.
There are imitation for blocking action. Different methods calls will run with random delay: from 1 to 5 seconds per call.
If you want to see how "deferred" workflow works click here.
There are imitation for asynchronous action. You will get "job id" and you can track the status in another endpoint.
Logic for workflow will be same as "complicated" workflow.
```

Also, you can open Temporal admin panel the located in [http://localhost:8088](http://localhost:8088/)

## Contribution

You are welcome to add more examples, fix bugs or orthographic errors.

## Useful links

#### Used libraries
[BaldinofRoadRunnerBundle](https://github.com/Baldinof/roadrunner-bundle)
[Temporal PHP SDK](https://github.com/temporalio/sdk-php)
[RoadRunner](https://github.com/spiral/roadrunner)

#### Temporal:
[Temporal (temporal.io)](https://temporal.io/)

#### Workshops
1st part [Оркестрируй это! Описываем сложные бизнес процессы на PHP - Антон Титов](https://www.youtube.com/watch?v=0NCMEaFMj_M)

2nd part [Оркестрация и закон Мерфи: обрабатываем ошибки-бизнес процессов](https://www.youtube.com/watch?v=upL8o-OXYEc)

#### Application (after run on local machine)
[This application demo](http://localhost:8080/)

[Temporal admin panel](http://localhost:8088/)

