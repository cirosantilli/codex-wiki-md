# Weakly symmetric channel capacity

↑ **Parent:** [Channel capacity](channel-capacity.md)

For a [discrete memoryless channel](discrete-memoryless-channel.md) with $m$ output symbols, suppose every row of the [transition matrix](stochastic-matrix.md) is a [permutation](permutation.md) of every other row and all column sums agree. Such a [communication channel](communication-channel.md) has

$$
C=\log_2m-H(\text{one row}).
$$

The row [Shannon entropy](information-entropy-split.md) is the same for every input, so $H(Y\mid X)$ has that fixed value for every input [probability distribution](probability-distribution-split.md). The remaining term $H(Y)$ is at most $\log_2m$ by [maximum entropy on a finite alphabet](maximum-entropy-on-a-finite-alphabet.md).

A uniform input attains the bound. If there are $\ell$ input symbols, the total of all [transition probabilities](transition-probability.md) in the [matrix](matrix.md) is $\ell$; equal column sums must therefore each be $\ell/m$. Multiplication by the uniform input mass $1/\ell$ gives output mass $1/m$ in each column. Hence $H(Y)=\log_2m$, which proves the displayed formula. The [cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md), [binary symmetric channel capacity](binary-symmetric-channel-capacity.md), and [ternary symmetric channel capacity](ternary-symmetric-channel-capacity.md) are concrete applications of this symmetry calculation.

**Table of contents**

- [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
  - [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
  - [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)
- [Ternary symmetric channel capacity](ternary-symmetric-channel-capacity.md)

## ↑ Ancestors (6)

1. [Channel capacity](channel-capacity.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/c/solution.md)
