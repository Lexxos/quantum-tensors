# Quantum Tensors

[![npm version](https://badge.fury.io/js/quantum-tensors.svg)](https://badge.fury.io/js/quantum-tensors)
![License](https://img.shields.io/npm/l/quantum-tensors)
[![Build Status](https://travis-ci.com/Quantum-Game/quantum-tensors.svg?branch=master)](https://travis-ci.com/Quantum-Game/quantum-tensors)
[![Coverage Status](https://codecov.io/gh/Quantum-Game/quantum-tensors/branch/master/graph/badge.svg)](https://codecov.io/gh/Quantum-Game/quantum-tensors/)
[![Twitter @QuantumGameIO](https://img.shields.io/twitter/follow/QuantumGameIO)](https://twitter.com/quantumgameio)

It is a JavaScript / TypeScript package for sparse tensor operations on complex numbers.
For example for quantum computing, quantum information, and well - the Quantum Game.

`(1.00 +0.00i) |1,2,>,V⟩` -> `(-0.71 +0.00i) |1,2,>,H⟩ + (0.71 +0.00i) |1,2,>,V⟩`

Developed at the [Centre of Quantum Technologies](https://www.quantumlah.org/), National University of Singapore, by [Piotr Migdał](https://p.migdal.pl/), [Philippe Cochin](https://github.com/sneakyweasel) et al.
It is a part of the [Quantum Game 2](https://github.com/Quantum-Game/quantum-game-2) project.

We base the philosophy of this package on:

* Sparse operations (both for vectors and matrices)
* Complex numbers
* Tensor structure 
* Named tensor dimensions (vide [Tensors considered harmful](http://nlp.seas.harvard.edu/NamedTensor)): there is a difference between a 2x2 operator on spin and polarization. It helps with catching errors.

Documentation: [quantum-game.github.io/quantum-tensors](https://quantum-game.github.io/quantum-tensors/) (generated by [TypeDoc](https://typedoc.org/)).

![Quantum Tensors logo](imgs/quantum-tensors-logo.jpg)

## Installation

The easiest way is to install from [the NPM repository](https://www.npmjs.com/package/quantum-tensors):

```
npm install quantum-tensors
```

Or, if you use [yarn](https://yarnpkg.com/) package manager, 

```
yarn add quantum-tensors
```

If you want to install a development version, you can get this package directly from this GitHub repository. In this case, the commands are:

```
npm install Quantum-Game/quantum-tensors#master
```

Or if you use yarn:

```
yarn add Quantum-Game/quantum-tensors#master
```

## Usage

And then in your project write:

```{ts}
import * as qt from 'quantum-tensors'
```

There are a few examples in [demos](https://github.com/Quantum-Game/quantum-tensors/tree/master/demos) folder.

## Why

For "Quantum Game 2" we needed a fast and precise way to simulate quantum stuff, so after tinkering with [mathjs](https://mathjs.org/) and [TensorFlow.js](https://www.tensorflow.org/js) we decided to code what we need from scratch.
At some point, we may want to use one of these libraries for backend, if we discover that it helps.

Also, [https://github.com/stared/thinking-in-tensors-writing-in-pytorch](https://github.com/stared/thinking-in-tensors-writing-in-pytorch) by Piotr Migdał.

## Contributing

* Create [TSDoc](https://www.npmjs.com/package/@microsoft/tsdoc) for each new function, class, and method
* Setup [ESLint](https://eslint.org/) configured as in this `.eslintrc.js` 
* Try to adhere to [Angular-like commit style](https://github.com/angular/angular/blob/master/CONTRIBUTING.md)

A few insights on contributing, and starting your projects, are in [How I Learned to Stop Worrying and Love the Types & Tests: the Zen of Python for TypeScript](https://p.migdal.pl/2020/03/02/types-tests-typescript.html) by Piotr Migdał.

## Interesting ideas

* A better notation (e.g. `⨂(op1, opt2, op3)`)
* An equation viewer

