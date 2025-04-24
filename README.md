# Generalized Harmonic Numbers Calculator

This program calculates the nth generalized harmonic number of order r, as defined by the formula: H(n, r) = 1/1<sup>r</sup> + 1/2<sup>r</sup> + ... + 1/n<sup>r</sup>

## Usage

Compile and run the program with two integer command-line arguments:
1. `n`: The upper bound of the summation (must be a positive integer)
2. `r`: The exponent used in the denominator terms

```bash
javac GeneralizedHarmonic.java
java GeneralizedHarmonic n r
```

## Examples

```bash
$ java GeneralizedHarmonic 1 1
1.0

$ java GeneralizedHarmonic 2 1
1.5

$ java GeneralizedHarmonic 3 2
1.3611111111111112
```

## Implementation Details

The program:
1. Takes two integer command-line arguments `n` and `r`
2. Uses a `for` loop to compute the sum of 1/k<sup>r</sup> for k from 1 to n
3. Prints the resulting generalized harmonic number as a double value

## Mathematical Background

Generalized harmonic numbers are related to the Riemann zeta function, which is important in number theory. The standard harmonic numbers are a special case where r = 1.

## Note

The program assumes that:
- `n` is a positive integer
- `r` can be any integer (though mathematically, it's typically considered for r > 0)
