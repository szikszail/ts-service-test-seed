# LM TS API testing PoC

## Prerequisites

1. NodeJS LTS (12+)
1. Yarn (`npm i -g yarn`)
1. Installed and running [ts-service-test-seed-service](https://github.com/szikszail/ts-service-test-seed-service) service

## Install

```console
yarn
```

## Running tests

```console
yarn test
```

To run the tests and open HTML report after the run:

```console
yarn test:e2e
```

## Reporting

During the test execution, the current progress is printed in the console and in the meantime the **Allure** report data is created.

Also, a **JUnit XML** report is generated to `junit.xml` file.

To create HTML report from the **Allure** report data:

```console
yarn report:generate
```

To open the generated HTML report:

```console
yarn report:open
```

**OR** to simply serve a temporary HTML report, without generating a final report:

```console
yarn report:server
```