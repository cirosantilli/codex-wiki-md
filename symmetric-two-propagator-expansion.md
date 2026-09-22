# Symmetric two-propagator expansion

↑ **Parent:** [Scalar bubble integral](scalar-bubble-integral.md)

Set $A=p^2-m^2\ne0$. The denominator product is exactly $(A+k^2)^2-4(p\cdot k)^2$. Its reciprocal therefore has the [Taylor expansion](taylor-expansion.md)

$$
\frac1{[(p-k)^2-m^2][(p+k)^2-m^2]}
=\frac1{A^2}\left[1-\frac{2k^2}{A}+\frac{4(p\cdot k)^2}{A^2}+O(k^4)\right].
$$

The coefficients follow by expanding $1/(1+x)=1-x+O(x^2)$ with $x=2k^2/A-4(p\cdot k)^2/A^2+O(k^4)$. The expansion is a local algebraic statement away from denominator zeros; integrating it through [Feynman propagator](feynman-propagator.md) poles requires a regulator and the correct [Feynman i-epsilon prescription](feynman-i-epsilon-prescription.md).

## ↑ Ancestors (8)

1. [Scalar bubble integral](scalar-bubble-integral.md)
2. [Bubble diagram](bubble-diagram.md)
3. [Feynman diagram](feynman-diagram.md)
4. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
5. [Quantum field theory](quantum-field-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
