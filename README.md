# faogustavo/ktlint-action-setup

This action installs ktlint.

## Input

```yml
inputs:
  ktlint_version:
    description: 'KTLint version.'
    default: '0.42.1'
```

## Usage

To run the KTLint action, you need to use a linux machine.

```yml
runs-on: ubuntu-latest
```

#### Default

```yml
steps:
  - uses: faogustavo/ktlint-action-setup@v1
  - run: ktlint --version
```


#### Specify ktlint version

```yml
steps:
  - uses: faogustavo/ktlint-action-setup@v1
    with:
        ktlint_version: 0.40.0
  - run: ktlint --version
```