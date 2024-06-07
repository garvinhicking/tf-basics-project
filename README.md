# TYPO3 Basics - testing-framework integration demo project

THIS IS A DUMMY PROJECT, forked from: https://github.com/sbuerk/tf-basics-project
Please read the original README.

!!! DO NOT USE FOR PRODUCTION !!!

# Ch-ch-changes

This is an example TYPO3 project which uses the normal TYPO3 testing-framework.

It is enhanced to use the https://github.com/garvinhicking/typo3-tf-runtests
(`garvinhicking/typo3-tf-runtests` composer package) to provide a
`runTests.sh` integration. That package simulates the `typo3/typo3` core
monorepository; the composer package would be a subtree-split of the `Build/Scripts/`
directory.

This dummy project assumes you know what you're doing. This is not
intended for production use.

# How to use?

- `composer install`
- `./vendor/bin/runTests.sh -s unit`
- `./vendor/bin/runTests.sh -s custom -- myStan`
- Marvel at science

# What and how?!

All variables for `runTests.sh` are configured in `runTests.env` of the project root.

You could specify a different location if you execute the runner differently:

```bash
RUNTESTS_ENV=./path/to/some/directory/with/runTest.env \
  ./vendor/bin/runTests.sh -s unit
```

