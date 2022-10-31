# Gradient Descent Matrix Decompositions

An experiment to see if one can decompose a matrix into the matrix multiplication of two matrixes through gradient descent.

See [decomp.ipynb](./decomp.ipynb) for the notebook

## Methodology

Lets say u wanna decompose matrix A which is a MxN matrix into a MxZ matrix (B) * a ZxN matrix (C).

I propose the following stupid algorithm, aptly named bogodecomp, for such a decomposition:

1. create a nerual network which has two linear layers and is just input * B * C
2. get training data of X = rand() and Y = AX
3. train the BC nn on that training data using gradient descent
4. bing bang boom BC=A

## Why

[@anish-lakkapragada](https://github.com/anish-lakkapragada) has been destroying my sleep schedule with ML math. I now think about ML in my sleep.

Send help

![i need answers](./img/needanswers.jpg)

## Results

It work

## Future

Stuff imma figure out later:

* does this work for matmul of 3 matrixes
* how many possible decompositions are there
* does this method accidentally yield a special factorization such as QR

## Citation

If you are using this in a paper, u probably goofed somewhere.

If you didn't, please contact me via [lichess direct message](https://lichess.org/@/r2d2bb8).