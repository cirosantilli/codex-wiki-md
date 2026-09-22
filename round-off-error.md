# Round-off error

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

[Round-off error](round-off-error.md) arises when numbers or arithmetic results are rounded to a finite set of representable values. Its scale is associated with [machine epsilon](machine-epsilon.md), and its effects depend on subsequent operations. Even a formula with zero [truncation error](truncation-error.md) can lose information. In decimal arithmetic rounded to three significant digits, $1.234$ becomes $1.23$ and $1.233$ becomes $1.23$: subtracting the stored numbers gives zero although the exact difference is $0.001$. The subtraction exposes errors already present in its nearly equal operands.

This example also has a large [condition number](condition-number.md): independently perturbing the two inputs of $a-b$ can produce a relative amplification $(|a|+|b|)/|a-b|=2467$. High sensitivity belongs to the input-output problem; [numerical stability](stability-of-a-numerical-method.md) concerns the arithmetic used to solve it. Conversely, on a common binary system with 53 significant bits and rounding to nearest, $(10^{16}+1)-10^{16}$ evaluates to zero while $(10^{16}-10^{16})+1$ evaluates to one. Exact arithmetic makes both one: changing summation order changes the accumulated [roundoff error](round-off-error.md). MIT's summation lecture explains why [numerical stability](stability-of-a-numerical-method.md) and the [condition number](condition-number.md) must be assessed separately.[Steven G. Johnson, MIT 18.335J, Lecture 3: Floating-Point Summation and Backwards Stability, 2019](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/pages/week-2/)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Matrix-chain cost model](matrix-chain-cost-model.md)
- [Round-off error](round-off-error.md)
