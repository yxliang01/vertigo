# vertigo
[![Build Status](https://travis-ci.org/JoranHonig/vertigo.svg?branch=master)](https://travis-ci.org/JoranHonig/vertigo)

Vertigo is a mutation testing framework designed to work specifically for smart contracts.
This mutation testing framework implements a range of mutation operators that are either selected from previous works or tailored to solidity.

### Quick Start Guide

To install vertigo, execute the following command:
```bash
pip3 install --user eth-vertigo
```

You can now run vertigo on a truffle project with the following command (assuming you have a `development` network configured in your`truffle-config.js`):

```bash
vertigo run --network development
```
Depending on your environment it might be required to specify the location of the truffle executable:
```bash
vertigo run --network development --truffle <node_dir>/bin/truffle 
```

There are a few additional parameters available that allow you to tweak the execution of vertigo:
```bash
$ vertigo run --help                                                                                                                                                ⬡ 9.11.2 [±master ●●▴]
Usage: vertigo run [OPTIONS]

  Performs a mutation test campaign

Options:
  --output TEXT            Output mutation test results to file
  --network TEXT           Network names that vertigo can use
  --truffle-location TEXT  Location of truffle cli
  --sample-ratio FLOAT     If this option is set. Vertigo will apply the
                           sample filter with the given ratio
  --exclude TEXT           Vertigo won't mutate files in these directories
  --help                   Show this message and exit.
                                                       
```
### Publications and Articles
[Practical Mutation Testing for Smart Contracts](https://link.springer.com/chapter/10.1007/978-3-030-31500-9_19) - Joran J. Honig, Maarten H. Everts, Marieke Huisman

[Introduction into Mutation Testing](https://medium.com/swlh/introduction-into-mutation-testing-d6512dc702b0?source=friends_link&sk=2878e0c08b6301a125198a264e43edb4) - Joran Honig

If you want to cite vertigo, please use the following:
```
@InProceedings{10.1007/978-3-030-31500-9_19,
author="Honig, Joran J.
and Everts, Maarten H.
and Huisman, Marieke",
title="Practical Mutation Testing for Smart Contracts",
booktitle="Data Privacy Management, Cryptocurrencies and Blockchain Technology",
year="2019",
publisher="Springer International Publishing",
pages="289--303",
```
